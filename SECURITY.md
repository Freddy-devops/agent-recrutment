---

**`SECURITY.md`**

```markdown
# HR Security Policy & Data Privacy Standards

This multi-agent recruitment pipeline enforces strict candidate data protection standards, prompt defense mechanisms, and automated legal compliance.

## 🛡️ Core Security Architecture

### 1. Resume Input Sanitization (Anti-Prompt Injection)
Unstructured text from candidates (CVs, cover letters, emails) is treated as untrusted data.
* Payloads are enclosed within explicit boundary tags (`<candidature_entrante>`).
* Screening agents run under explicit security directives preventing execution of embedded system overrides (`SYSTEM OVERRIDE`).

### 2. Candidate Data Sovereignty & Isolation
* **Tenant Partitioning**: Each client organization and applicant profile is isolated by unique tenant identifiers.
* **Right to be Forgotten (GDPR)**: The `kill_switch_rgpd_rh` function provides surgical deletion of candidate records within 24 hours of request, preserving overall database integrity.

### 3. Algorithmic Transparency (EU AI Act & EEOC)
* **EU AI Act Transparency**: Automated emails sent to candidate locations within the European Union automatically append mandatory notices of AI-assisted processing.
* **Non-Discriminatory Evaluation**: Qualification agents evaluate strictly against explicit technical criteria to uphold objective recruitment practices.

## 🔒 Vulnerability Reporting

To report a vulnerability or compliance issue, contact `beyamfred@gmail.com`. Reports are prioritized and addressed immediately.