<p align="center">
  <img src="https://avatars.githubusercontent.com/u/204997969?v=4" width="120" />
</p>

<h1 align="center">Lambdasistemi</h1>

<p align="center"><em>Good practices for fun and profit</em></p>

<p align="center">Haskell &middot; Cardano &middot; Nix &middot; PureScript</p>

---

### Cardano Infrastructure

| Repository | Description | Pages |
|---|---|---|
| [cardano-utxo-csmt](https://github.com/lambdasistemi/cardano-utxo-csmt) | Compact Sparse Merkle Tree over Cardano's UTxO set for inclusion proofs | [docs](https://lambdasistemi.github.io/cardano-utxo-csmt/) |
| [cardano-node-clients](https://github.com/lambdasistemi/cardano-node-clients) | Haskell clients for Cardano node mini-protocols (N2C + N2N) | [docs](https://lambdasistemi.github.io/cardano-node-clients/) |
| [cardano-mithril-client](https://github.com/lambdasistemi/cardano-mithril-client) | Haskell client for Mithril UTxO snapshot download, verification, and extraction | |
| [cardano-read-ledger](https://github.com/lambdasistemi/cardano-read-ledger) | Read Cardano block data, parametrized by era | [docs](https://lambdasistemi.github.io/cardano-read-ledger/) |
| [chain-follower](https://github.com/lambdasistemi/chain-follower) | Abstract chain follower types — Follower, Intersector, ProgressOrRewind | [docs](https://lambdasistemi.github.io/chain-follower/) |
| [cardano-ledger-inspector](https://github.com/lambdasistemi/cardano-ledger-inspector) | Cardano ledger operations compiled to WASI for browser and CLI tooling | |
| [amaru-treasury-tx](https://github.com/lambdasistemi/amaru-treasury-tx) | Build unsigned Amaru treasury transactions (disburse, reorganize, withdraw) | |
| [amaru-bootstrap](https://github.com/lambdasistemi/amaru-bootstrap) | Bootstrap data pipeline for Amaru on custom Cardano testnets — uses stock IOG tools, no consensus fork | |
| [cardano-stake-csmt](https://github.com/lambdasistemi/cardano-stake-csmt) | CSMT over per-epoch Cardano stake distribution — verifiable stake-weighted voting proofs | [docs](https://lambdasistemi.github.io/cardano-stake-csmt/) |
| [cardano-ledger-wasm](https://github.com/lambdasistemi/cardano-ledger-wasm) | Cardano ledger operations compiled to wasm32-wasi | |
| [cardano-testnet-baker](https://github.com/lambdasistemi/cardano-testnet-baker) | Deterministic Cardano testnet artifact baker — genesis, keys, and ChainDB seeds from declarative JSON | |
| [cip113-tx-builder](https://github.com/lambdasistemi/cip113-tx-builder) | CIP-113 programmable token transaction builders — CLI, Haskell library, WASM-WASI | [docs](https://lambdasistemi.github.io/cip113-tx-builder/) |

### Merkle Patricia Forestry

| Repository | Description | Pages |
|---|---|---|
| [cardano-mpfs-offchain](https://github.com/lambdasistemi/cardano-mpfs-offchain) | Fact CRUD, transaction building, devnet server for MPFS on Cardano | [docs](https://lambdasistemi.github.io/cardano-mpfs-offchain/) |
| [cardano-mpfs-browser](https://github.com/lambdasistemi/cardano-mpfs-browser) | MPFS fact explorer, transaction viewer and signer | [app](https://lambdasistemi.github.io/cardano-mpfs-browser/) |
| [haskell-mts](https://github.com/lambdasistemi/haskell-mts) | Merkle Trees in Haskell with persistent storage and proofs | [docs](https://lambdasistemi.github.io/haskell-mts/) |

### Wallets & Signing

| Repository | Description | Pages |
|---|---|---|
| [cardano-wallet-sign](https://github.com/lambdasistemi/cardano-wallet-sign) | Cardano BIP39 wallet derivation and transaction signing library | |
| [cardano-swiss-knife](https://github.com/lambdasistemi/cardano-swiss-knife) | Browser-first Cardano Swiss Knife for address tools, transaction inspection, and detached witness signing | |
| [cardano-addresses-browser](https://github.com/lambdasistemi/cardano-addresses-browser) | Browser-based Cardano address toolkit — PureScript replacement for cardano-addresses CLI | |
| [haskell-gamechanger](https://github.com/lambdasistemi/haskell-gamechanger) | Haskell client for the GameChanger Cardano wallet — script DSL, URL encoding, callback handling | |
| [cardano-tx-tools](https://github.com/lambdasistemi/cardano-tx-tools) | Cardano transaction tooling — builder, structural diff, blueprint decoding | [docs](https://lambdasistemi.github.io/cardano-tx-tools/) |
| [cardano-wallet-tools](https://github.com/lambdasistemi/cardano-wallet-tools) | Operator wallet-UTxO toolkit + PureScript CIP-30 browser wallet over cardano-tx-tools | [docs](https://lambdasistemi.github.io/cardano-wallet-tools/) |
| [cardano-multisig](https://github.com/lambdasistemi/cardano-multisig) | Permissionless witness-collection backend for Conway transactions — signature-authorized, accountless, self-cleaning | |

### Zero-Knowledge

| Repository | Description | Pages |
|---|---|---|
| [harvest](https://github.com/lambdasistemi/harvest) | ZK voucher system for Cardano using Groth16 proofs | |
| [zk-lab](https://github.com/lambdasistemi/zk-lab) | Lab for intention-driven zero-knowledge DSL targeting Plutus (Groth16, BBS+, Halo2) | |
| [cardano-bbs](https://github.com/lambdasistemi/cardano-bbs) | BBS+ anonymous credentials for Cardano — Haskell off-chain + Aiken on-chain | |
| [peer-proof-protocols](https://github.com/lambdasistemi/peer-proof-protocols) | Research and specifications for peer-only Merkle proof protocols | |

### Credentials & Compliance

| Repository | Description | Pages |
|---|---|---|
| [cardano-vcr](https://github.com/lambdasistemi/cardano-vcr) | W3C Verifiable Credentials 2.0 on Cardano via MPFS | [docs](https://lambdasistemi.github.io/cardano-vcr/) |
| [eu-digital-product-passport](https://github.com/lambdasistemi/eu-digital-product-passport) | Feasibility study: EU Digital Product Passports on Cardano | [docs](https://lambdasistemi.github.io/eu-digital-product-passport/) |
| [cardano-for-regulators](https://github.com/lambdasistemi/cardano-for-regulators) | Mapping multi-party regulations to Cardano compliance infrastructure | [docs](https://lambdasistemi.github.io/cardano-for-regulators/) |
| [cddl-aiken](https://github.com/lambdasistemi/cddl-aiken) | CDDL to Aiken withdrawal validator compiler | [docs](https://lambdasistemi.github.io/cddl-aiken/) |

### Governance & Knowledge Graphs

| Repository | Description | Pages |
|---|---|---|
| [cardano-knowledge-maps](https://github.com/lambdasistemi/cardano-knowledge-maps) | Interactive knowledge graph of Cardano governance (CIP-1694, Conway era) | [app](https://lambdasistemi.github.io/cardano-knowledge-maps/) |
| [graph-browser](https://github.com/lambdasistemi/graph-browser) | Interactive knowledge graph browser with guided tours — PureScript + Cytoscape.js | [app](https://lambdasistemi.github.io/graph-browser/) |
| [call-graph-explorer](https://github.com/lambdasistemi/call-graph-explorer) | Interactive function call graph explorer for Haskell projects | [app](https://lambdasistemi.github.io/call-graph-explorer/) |
| [cardano-ledger-rdf](https://github.com/lambdasistemi/cardano-ledger-rdf) | Cardano transaction graph and RDF tools | [docs](https://lambdasistemi.github.io/cardano-ledger-rdf/) |
| [cardano-rdf-registry](https://github.com/lambdasistemi/cardano-rdf-registry) | Trustless MPFS-rooted registry for RDF books — owner-bound naming, content-addressed, offline-verified | |

### KERI

| Repository | Description | Pages |
|---|---|---|
| [cardano-keri](https://github.com/lambdasistemi/cardano-keri) | KERI AID on Cardano — self-certifying identifiers with pre-rotation for on-chain credential anchoring | [docs](https://lambdasistemi.github.io/cardano-keri/) |
| [kel-circle](https://github.com/lambdasistemi/kel-circle) | Synchronized multi-KEL circle protocol — event-sourced group coordination | [docs](https://lambdasistemi.github.io/kel-circle/) |

### Developer Tooling

| Repository | Description | Pages |
|---|---|---|
| [agent-daemon](https://github.com/lambdasistemi/agent-daemon) | WebSocket daemon for managing Claude Code agent sessions via tmux and git worktrees | [docs](https://lambdasistemi.github.io/agent-daemon/) |
| [kanbanned](https://github.com/lambdasistemi/kanbanned) | Terminal kanban board for agent-daemon | |
| [gh-dashboard](https://github.com/lambdasistemi/gh-dashboard) | Client-side GitHub dashboard — repos, issues, PRs, projects and CI on a single page | [app](https://lambdasistemi.github.io/gh-dashboard/) |
| [libvterm-haskell](https://github.com/lambdasistemi/libvterm-haskell) | Haskell FFI bindings to libvterm (neovim fork) | |
| [homebrew-tap](https://github.com/lambdasistemi/homebrew-tap) | Homebrew formulae for lambdasistemi projects | |
| [cachix-warmup](https://github.com/lambdasistemi/cachix-warmup) | Cachix cache warming workflows for GHC on aarch64-darwin | |

### Libraries

| Repository | Description | Pages |
|---|---|---|
| [rocksdb-haskell](https://github.com/lambdasistemi/rocksdb-haskell) | RocksDB Haskell bindings | |
| [rocksdb-kv-transactions](https://github.com/lambdasistemi/rocksdb-kv-transactions) | RocksDB backend for key-value transactions | [docs](https://lambdasistemi.github.io/rocksdb-kv-transactions/) |
| [contra-tracer-contrib](https://github.com/lambdasistemi/contra-tracer-contrib) | Utility modules for contra-tracer: file logging, thread-safe wrappers, timestamps, throttling | [docs](https://lambdasistemi.github.io/contra-tracer-contrib/) |
| [crypton-certificate](https://github.com/lambdasistemi/crypton-certificate) | Certificate and Key Reader/Writer in Haskell | |
| [datastar-haskell-nix](https://github.com/lambdasistemi/datastar-haskell-nix) | Nix flake wrapper for datastar-haskell (GHC 9.12.2) | |
| [datastar-examples](https://github.com/lambdasistemi/datastar-examples) | TODO list app with datastar-hs, Warp, SQLite, Pico CSS | |

### Other

| Repository | Description | Pages |
|---|---|---|
| [giacenza](https://github.com/lambdasistemi/giacenza) | | [page](https://lambdasistemi.github.io/giacenza/) |
| [antithesing-1](https://github.com/lambdasistemi/antithesing-1) | Antithesis testing repository | |
