# Integration Map

How components connect and what data flows between them.

### Frontend-scaffold --> Openclaw-agent

- **Source**: Frontend-scaffold (`1f88ad43`)
  - Output ports: App Context (config)
- **Target**: Openclaw-agent (`08509c38`)
  - Input ports: Agent Prompt (config)

### Stylus-rust-contract --> Smartcache-caching

- **Source**: Stylus-rust-contract (`304ff36c`)
  - Output ports: Contract Code (contract)
- **Target**: Smartcache-caching (`bbeb4614`)
  - Input ports: Contract Input (contract)

### Stylus-rust-contract --> Auditware-analyzing

- **Source**: Stylus-rust-contract (`304ff36c`)
  - Output ports: Contract Code (contract)
- **Target**: Auditware-analyzing (`b7960b96`)
  - Input ports: Contract Input (contract)

### Stylus-rust-contract --> Frontend-scaffold

- **Source**: Stylus-rust-contract (`304ff36c`)
  - Output ports: Contract Code (contract)
- **Target**: Frontend-scaffold (`1f88ad43`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Smartcache-caching --> Auditware-analyzing

- **Source**: Smartcache-caching (`bbeb4614`)
  - Output ports: Cached Contract (contract)
- **Target**: Auditware-analyzing (`b7960b96`)
  - Input ports: Contract Input (contract)

### Frontend-scaffold --> Wallet-auth

- **Source**: Frontend-scaffold (`1f88ad43`)
  - Output ports: App Context (config)
- **Target**: Wallet-auth (`be90ed53`)
  

### Frontend-scaffold --> Rpc-provider

- **Source**: Frontend-scaffold (`1f88ad43`)
  - Output ports: App Context (config)
- **Target**: Rpc-provider (`f943dadc`)
  

### Frontend-scaffold --> Dune-transaction-history

- **Source**: Frontend-scaffold (`1f88ad43`)
  - Output ports: App Context (config)
- **Target**: Dune-transaction-history (`84553149`)
  

### Stylus-rust-contract --> Chainlink-price-feed

- **Source**: Stylus-rust-contract (`304ff36c`)
  - Output ports: Contract Code (contract)
- **Target**: Chainlink-price-feed (`5ad21144`)
  

### Erc1155-stylus --> Smartcache-caching

- **Source**: Erc1155-stylus (`4b63f83b`)
  - Output ports: Multi-Token Contract (contract)
- **Target**: Smartcache-caching (`bbeb4614`)
  - Input ports: Contract Input (contract)
