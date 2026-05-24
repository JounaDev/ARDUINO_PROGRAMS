# SECURITY.md — Security Policy

**Project Maintainer:** Jounadev  
**Security Program Level:** Production-Grade Controlled Disclosure Policy  
**Last Updated:** 2026-05-24

---

# 1. Supported Versions

Only actively maintained versions receive security updates, patches, and hotfixes.

| Version Range | Status               | Security Support |
|--------------|---------------------|------------------|
| 2.0.x        | Stable (current)     | :white_check_mark: |
| 1.5.x        | Legacy LTS           | :white_check_mark: |
| 1.0.x        | Deprecated           | :x:               |
| < 1.0        | End of Life (EOL)    | :x:               |

> ⚠️ End-of-life versions are considered unsafe and may contain known vulnerabilities.

---

# 2. Security Principles

This project follows strict security principles:

- **Least privilege execution model**
- **No trust of external inputs by default**
- **Input validation at all system boundaries**
- **Defense-in-depth architecture**
- **Tamper-aware design where applicable**
- **Deterministic execution for critical modules**

---

# 3. Vulnerability Classification (Severity Model)

We classify vulnerabilities using a CVSS-inspired internal model:

| Severity | Impact Description | Response Time |
|----------|-------------------|---------------|
| CRITICAL | Remote code execution, system compromise, data breach | 24–72 hours |
| HIGH     | Privilege escalation, major logic bypass | 3–5 days |
| MEDIUM   | Partial data exposure, non-critical bypass | 7–14 days |
| LOW      | Minor issues, non-exploitable weaknesses | Next release cycle |
| INFO     | Hardening suggestions | Optional |

---

# 4. Reporting a Vulnerability

We strongly encourage **responsible disclosure**.

## 📩 Secure Reporting Channels

Report vulnerabilities privately via:

- Email: security@jounadev.dev *(recommended)*
- Encrypted channel (if available)
- Private project contact channel

> DO NOT disclose vulnerabilities publicly before coordination.

---

# 5. What to Include in a Report

To accelerate triage, include:

- Clear description of the vulnerability
- Affected version(s)
- Steps to reproduce
- Proof of concept (PoC) if possible
- Potential impact analysis
- Suggested mitigation (optional)

---

# 6. Response Lifecycle

Once a report is submitted:

### Phase 1 — Acknowledgement
- Response within **48–72 hours**
- Ticket is created and tracked internally

### Phase 2 — Validation
- Security team verifies reproducibility
- Severity classification assigned

### Phase 3 — Remediation
- Patch development begins
- Hotfix or scheduled release depending on severity

### Phase 4 — Disclosure Coordination
- Reporter is credited (if desired)
- Public advisory released after fix is deployed

---

# 7. Disclosure Policy

We follow **Coordinated Vulnerability Disclosure (CVD)**:

- No public disclosure until patch is available
- Embargo period may apply for critical issues
- Researchers are expected to avoid exploitation or data access beyond PoC scope

---

# 8. Out of Scope

The following are NOT considered vulnerabilities:

- Theoretical attacks without proof of exploitability
- Social engineering against users
- Physical attacks on infrastructure
- Issues in unsupported third-party dependencies (unless exploitable within system context)
- Misconfiguration outside documented deployment model

---

# 9. Security Rewards (Optional / Future Program)

A bounty program may be introduced in future versions:

- Critical: reward tier A
- High: reward tier B
- Medium: reward tier C

(Currently not active unless explicitly announced)

---

# 10. Legal Protection Clause

Unauthorized access, exploitation, reverse engineering, or tampering
with security mechanisms may result in:

- Permanent restriction from system access
- Legal action under applicable cybersecurity laws
- Blacklisting from future services

---

# 11. Security Philosophy

Security is not a feature — it is a system constraint.

All contributions must respect the integrity of the architecture.

---

© 2026 Jounadev — Security Division
All rights reserved.
