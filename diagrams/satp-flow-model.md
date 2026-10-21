
---

# 📁 **diagrams/satp-flow-model.md**

```markdown
# SATP Flow Governance Model (Mermaid)

```mermaid
sequenceDiagram
    participant Entity
    participant SATP
    participant Policy
    participant AI

    Entity->>SATP: Initiate Flow
    SATP->>Policy: Evaluate Trust & Context
    Policy->>SATP: Allow / Deny / Constrain
    SATP->>AI: Telemetry & Evidence
    AI->>SATP: Reasoning & Recommendations
    SATP->>Entity: Enforce Decision
