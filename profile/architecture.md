graph TD

  subgraph INPUT["  ⬛  INPUT LAYER"]
    direction TB
    U(["👤  User / External Request"])
  end

  subgraph INTERFACE["  🔷  INTERFACE & INFERENCE LAYER"]
    direction LR
    OS["🖥️  prano-os
    ─────────────────
    Orchestration & API Gateway
    Route · Dispatch · Respond"]

    UNIFIED["🔐  prano-sovereign-unified
    ─────────────────
    Secure Inference & Multi-Node
    Communication Bus"]
  end

  subgraph CORE["  🧠  INTELLIGENCE CORE LAYER"]
    direction LR
    KERNEL["⚙️  prano-sovereign-kernel
    ─────────────────
    Core AI Engine · Decision Logic
    Process Manager · R=1 Evaluator"]

    VAULT["🗄️  prano-intelligence-vault
    ─────────────────
    Knowledge Base · RAG Memory
    Genkit Context Store"]

    PROTO["🧪  gemma-protocol-phase-zero
    ─────────────────
    Local Model Validation
    Offline Protocol · Integrity Gate"]
  end

  subgraph GOVERNANCE["  🏛️  GOVERNANCE & CONTROL LAYER"]
    direction LR
    SYSTEM["🗂️  prano-sovereign-system
    ─────────────────
    Unified Control · Version Alignment
    Backup Orchestration"]

    EMPIRE["👑  neamah-empire
    ─────────────────
    Strategic Command · Investment Ops
    Governance Policies"]
  end

  subgraph EXECUTION["  ⚡  EXECUTION LAYER"]
    direction TB
    FIELD["🚜  neamah-field-operations
    ─────────────────
    Field Execution · Live Data Collection
    Kinetic Operations Tracker"]
  end

  U -->|"HTTP / WebSocket Request"| OS
  UNIFIED <-->|"Encrypted Multi-Node Channel"| OS
  OS -->|"Dispatch Intelligence Job"| KERNEL
  KERNEL <-->|"Read / Write Context"| VAULT
  PROTO -->|"Validation Signal · R=1 Gate"| KERNEL
  KERNEL -->|"Processed Decision Output"| SYSTEM
  SYSTEM -->|"Policy · Command Feed"| EMPIRE
  EMPIRE -->|"Operational Orders"| FIELD
  VAULT -.->|"Knowledge Enrichment"| FIELD

  classDef inputNode   fill:#1a1a2e,stroke:#e94560,color:#fff
  classDef ifaceNode   fill:#16213e,stroke:#0f3460,color:#a8d8ea
  classDef coreNode    fill:#0f3460,stroke:#533483,color:#e2e2e2
  classDef govNode     fill:#533483,stroke:#e94560,color:#fff
  classDef execNode    fill:#1b4332,stroke:#40916c,color:#d8f3dc

  class U inputNode
  class OS,UNIFIED ifaceNode
  class KERNEL,VAULT,PROTO coreNode
  class SYSTEM,EMPIRE govNode
  class FIELD execNode

  style INPUT      fill:#0d0d0d,stroke:#e94560,stroke-width:2px,color:#e94560
  style INTERFACE  fill:#0d1b2a,stroke:#0f3460,stroke-width:2px,color:#a8d8ea
  style CORE       fill:#0a1628,stroke:#533483,stroke-width:2px,color:#c77dff
  style GOVERNANCE fill:#1a0a28,stroke:#7b2d8b,stroke-width:2px,color:#e040fb
  style EXECUTION  fill:#0a1f0a,stroke:#40916c,stroke-width:2px,color:#74c69d
