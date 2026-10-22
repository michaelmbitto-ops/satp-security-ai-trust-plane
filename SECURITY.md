# Security Policy — SATP v1.1

The Security–AI Trust Plane (SATP) is a unified trust fabric designed to govern human, machine, and AI interactions across modern distributed systems. Because SATP includes identity, flow classification, guardrail enforcement, telemetry correlation, and AI reasoning components, responsible disclosure is essential to maintaining the integrity of the project and the safety of downstream users.

This document outlines how to report vulnerabilities, how disclosures are handled, and what to expect during the triage and remediation process.

---

## 📩 Reporting a Vulnerability

If you discover a security vulnerability in SATP, please report it privately via email:

📧 **michael.m.bitto@gmail.com**

Do **not** open public GitHub issues for security concerns.

You may also report vulnerabilities using GitHub’s private security advisory system:

👉 https://github.com/michaelmbitto-ops/satp-security-ai-trust-plane/security/advisories/new

Both channels are monitored. Responsible disclosure is appreciated and helps protect the SATP ecosystem and any systems built on top of it.

---

## 🔐 What to Include in Your Report

To help us triage effectively, please include:

- A clear description of the vulnerability  
- Steps to reproduce (if applicable)  
- Impact assessment (what could an attacker do?)  
- Affected SATP components (IEL, FCL, PGL, TEL, RAL, UCP, examples, etc.)  
- Any relevant logs, traces, or flow data  
- Whether the issue involves AI agent behavior or autonomous workflows  

SATP v1.1 introduces AI‑aware governance, so disclosures involving autonomous agents, delegated identity, or reasoning‑layer behavior are especially important.

---

## 🕒 Response & Triage Timeline

You can expect the following timeline:

- **Acknowledgment:** within 48 hours  
- **Initial triage:** within 5–7 days  
- **Severity classification:** within 7–10 days  
- **Fix or mitigation plan:** within 14 days (severity‑dependent)  
- **Coordinated disclosure:** as soon as a fix is available  

Critical issues may be addressed sooner depending on impact.

---

## 🧩 Severity Classification

SATP uses a flow‑centric severity model aligned with v1.1 architecture:

### **Critical**
- Compromise of identity or entity registry (IEL)  
- Unauthorized flow creation or flow manipulation (FCL)  
- Policy bypass or guardrail failure (PGL)  
- Evidence graph corruption or telemetry injection (TEL)  
- Malicious autonomous agent behavior or reasoning hijack (RAL)  

### **High**
- Unauthorized access to sensitive SATP APIs  
- Flow misclassification leading to incorrect policy enforcement  
- Trust score manipulation  

### **Medium**
- Denial‑of‑service conditions affecting SATP microservices  
- Incorrect flow context extraction  
- Non‑critical telemetry parsing issues  

### **Low**
- Minor validation errors  
- UI issues in the Unified Control Plane (UCP)  
- Documentation inaccuracies  

---

## 🧠 AI Agent & Autonomous Workflow Vulnerabilities

SATP v1.1 introduces explicit governance for:

- Autonomous agents  
- Delegated identity  
- Ephemeral identity  
- Multi‑agent workflows  
- AI reasoning and action enforcement  

If your vulnerability involves AI behavior, please specify:

- Whether the agent acted outside its guardrails  
- Whether delegated identity was misused  
- Whether reasoning‑layer decisions were incorrect  
- Whether flows were generated autonomously without proper classification  
- Whether trust scoring was affected  

These issues are treated with heightened priority.

---

## 🔄 Coordinated Disclosure

SATP follows responsible disclosure practices:

- Vulnerabilities are fixed privately before public announcement  
- Contributors who report issues may be credited (optional)  
- Public disclosure occurs only after patches or mitigations are available  
- Critical issues may involve coordinated release timing  

If you prefer anonymity, please state so in your report.

---

## 🛡️ Scope

This security policy applies to:

- SATP whitepaper and specifications  
- SATP reference implementation (Go microservices)  
- Unified Control Plane (UCP)  
- Flow schemas  
- Guardrail policies  
- Evidence graph logic  
- Reasoning & autonomy components  
- Examples and integrations  

It does **not** apply to external dependencies (e.g., OPA, OpenTelemetry, Neo4j, cloud providers).

---

## 📄 Version

**Security Policy Version:** 1.1  
Aligned with **SATP v1.1.0 — Unified Trust Plane Architecture & Whitepaper Overhaul**

---

## 🙏 Thank You

Thank you for helping keep SATP secure.  
Your contributions strengthen the trust fabric that governs human, machine, and AI interactions across modern distributed systems.
