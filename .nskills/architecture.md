# Architecture

## Dependency Graph

```mermaid
graph TD
  304ff36c["Stylus-rust-contract (stylus-rust-contract)"]
  4b63f83b["Erc1155-stylus (erc1155-stylus)"]
  1f88ad43["Frontend-scaffold (frontend-scaffold)"]
  5ad21144["Chainlink-price-feed (chainlink-price-feed)"]
  bbeb4614["Smartcache-caching (smartcache-caching)"]
  08509c38["Openclaw-agent (openclaw-agent)"]
  be90ed53["Wallet-auth (wallet-auth)"]
  f943dadc["Rpc-provider (rpc-provider)"]
  84553149["Dune-transaction-history (dune-transaction-history)"]
  b7960b96["Auditware-analyzing (auditware-analyzing)"]
  1f88ad43 --> 08509c38
  304ff36c --> bbeb4614
  304ff36c --> b7960b96
  304ff36c --> 1f88ad43
  bbeb4614 --> b7960b96
  1f88ad43 --> be90ed53
  1f88ad43 --> f943dadc
  1f88ad43 --> 84553149
  304ff36c --> 5ad21144
  4b63f83b --> bbeb4614
```

## Execution / Implementation Order

1. **Stylus-rust-contract** (`304ff36c`)
2. **Erc1155-stylus** (`4b63f83b`)
3. **Frontend-scaffold** (`1f88ad43`)
4. **Chainlink-price-feed** (`5ad21144`)
5. **Smartcache-caching** (`bbeb4614`)
6. **Openclaw-agent** (`08509c38`)
7. **Wallet-auth** (`be90ed53`)
8. **Rpc-provider** (`f943dadc`)
9. **Dune-transaction-history** (`84553149`)
10. **Auditware-analyzing** (`b7960b96`)
