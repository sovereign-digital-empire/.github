graph TD

%% USER LAYER
U[User / Input Layer]

%% CORE LAYER
OS[prano-os<br/>Orchestration Layer]
KERNEL[prano-sovereign-kernel<br/>Core Intelligence Engine]
VAULT[prano-intelligence-vault<br/>Memory & Knowledge Vault]

%% GOVERNANCE LAYER
SYSTEM[prano-sovereign-system<br/>Unified Control System]
EMPIRE[neamah-empire<br/>Governance & Command]

%% EXECUTION LAYER
FIELD[neamah-field-operations<br/>Execution & Operations Layer]

%% PROTOCOL LAYER
PROTO[gemma-protocol-phase-zero<br/>Validation & Protocol Layer]
UNIFIED[prano-sovereign-unified<br/>Secure Inference & Communication Layer]

%% FLOW
U --> OS
OS --> KERNEL
KERNEL --> VAULT

KERNEL --> SYSTEM
SYSTEM --> EMPIRE

EMPIRE --> FIELD
VAULT --> FIELD

PROTO --> KERNEL
UNIFIED --> OS
