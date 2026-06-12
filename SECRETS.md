# Org secret & token management

**Principle:** GitHub access for CI comes from **one org GitHub App**, not personal PATs.
Workflows mint a short-lived, repo-scoped token at runtime via
`actions/create-github-app-token`. The only long-lived GitHub secret is the App's
private key, stored **once at the org level** (and in 1Password as system-of-record).

## Inventory (2026-06-12 audit)

### GitHub credentials → migrate to the org App (`lambdasistemi-ci`)
| Secret | Where | Job |
|---|---|---|
| `TAP_TOKEN` | org + agent-daemon, amaru-treasury-tx, cardano-ledger-rdf, cardano-mpfs-offchain, cachix-warmup, cardano-tx-tools (7) | push Homebrew formula to `homebrew-tap` |
| `RELEASE_BOT_SSH_KEY` | amaru-treasury-tx, browser-json-tree, cardano-ledger-rdf, cardano-node-clients, cardano-tx-tools (5) | release-bot git push |
| `RELEASE_PLEASE_TOKEN` | haskell-mts | release-please PRs trigger CI |
| `RELEASE_BOT_TOKEN` | plutus | release automation |
| `GH_DASHBOARD_TOKEN` | gh-dashboard | read repos for the dashboard |

Seed App secrets live on `cardano-mpfs-offchain`: `TAP_APP_ID`, `TAP_APP_PRIVATE_KEY`
(to be promoted to org-level: id → org *variable* `CI_APP_ID`, key → org *secret* `CI_APP_PRIVATE_KEY`).

### Non-GitHub service tokens → de-duplicate to org-level
- `CACHIX_AUTH_TOKEN` — org `ALL` already covers everything; **25 repo copies are redundant, delete them**.
- `SURGE_TOKEN` / `SURGE_LOGIN` (9) — promote to org-level.

### Genuinely scoped — keep as-is
- `PROD_SSH_HOST/KEY/USER` (amaru-treasury-tx) — server deploy.
- `BLOCKFROST_PROJECT_ID` (cardano-ledger-inspector) — Blockfrost API id.

## How to add CI GitHub access to a new repo
1. Install the org App on the repo (Org → GitHub Apps → Configure).
2. In the workflow: `actions/create-github-app-token` with `app-id: ${{ vars.CI_APP_ID }}`,
   `private-key: ${{ secrets.CI_APP_PRIVATE_KEY }}`, `owner: lambdasistemi`, `repositories: <repo>`.
3. No new secret. The next fork adds zero tokens — that is the success test.
