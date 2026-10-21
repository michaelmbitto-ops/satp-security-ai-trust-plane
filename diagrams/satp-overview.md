# SATP Overview Diagram (Mermaid)

```mermaid
flowchart TD
    A[Entities] --> B[Flows]
    B --> C[Policy & Guardrails]
    C --> D[Telemetry & Evidence]
    D --> E[AI Reasoning]
    E --> C
    E --> B
