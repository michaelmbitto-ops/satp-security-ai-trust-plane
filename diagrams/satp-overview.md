# SATP Layer Model

```mermaid
graph TD
    IEL["Identity & Entity Layer"]
    FCL["Flow & Context Layer"]
    PGL["Policy & Guardrail Layer"]
    TEL["Telemetry & Evidence Layer"]
    RAL["Reasoning & Autonomy Layer"]

    IEL --> FCL --> PGL --> TEL --> RAL