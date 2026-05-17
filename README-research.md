# [TRACK-CODE] — Task [NN]: [Task Title]

> **Intern:** [Full Name] | **Track:** [Track Name] | **Cohort:** [N] | **Date:** YYYY-MM-DD
> **Difficulty:** [Beginner / Intermediate / Advanced] | **Duration:** [X Hours] | **Status:** [Complete / Partial]

---

## Executive Summary
<!-- 3–5 sentences for a non-technical reader, manager, or client.
     What environment or system was reviewed? What were the key findings?
     What is the most important recommendation?
     Example: "An AWS IAM configuration review was conducted across a simulated cloud environment.
     Three high-severity misconfigurations were identified that could allow privilege escalation
     and unauthorized data access. Immediate policy remediation and credential rotation are recommended." -->

---

## Assessment Scope

| Item | Detail |
|---|---|
| Assessment Type | [Configuration Review / Architecture Review / Risk Assessment / Threat Model / Compliance Mapping] |
| Environment / System | e.g. AWS Free Tier Account / Simulated Enterprise Network |
| Services / Components in Scope | |
| Out of Scope | |
| Framework / Standard Applied | e.g. AWS Well-Architected / CIS Benchmarks / NIST CSF / MITRE ATT&CK |
| Lab Platform | [AWS Free Tier / Azure / TryHackMe / Custom Lab] |
| Task Objective | [Copy from task description — one sentence] |

---

## Environment Setup
<!-- How did you access or configure the environment for this task?
     Include: cloud account setup, tools installed, services configured.
     Another intern must be able to replicate your environment exactly from these steps. -->

**Step 1:**
**Step 2:**
**Step 3:**

---

## Methodology

<!-- Which of these applied to this task? Tick all that apply. -->

- [ ] **Configuration Review** — Comparing settings against a security baseline or standard
- [ ] **Architecture Analysis** — Evaluating design decisions for security risk
- [ ] **Threat Modeling** — Identifying assets, threats, vulnerabilities, and attack paths
- [ ] **Risk Assessment** — Scoring and prioritizing identified risks
- [ ] **Access Review** — Evaluating identity, permissions, and trust relationships
- [ ] **Compliance Mapping** — Aligning controls to a regulatory or industry framework
- [ ] **Attack Surface Analysis** — Mapping exposure points from an attacker's perspective

**Process:**
<!-- Describe exactly what you did, in the order you did it.
     What did you review first? What tools or commands did you use to gather data?
     What framework or checklist guided your assessment? -->

---

## Architecture Overview

<!-- Describe or diagram the environment you assessed.
     What services/components exist? How do they connect?
     What are the trust boundaries and data flows? -->

**Environment Description:**

**Components Identified:**

| Component | Type | Role | Exposure Level |
|---|---|---|---|
| | | | Internal / External / Both |
| | | | |

> Architecture diagram: `diagrams/architecture-overview.png`
> Data flow diagram: `diagrams/data-flow.png`

---

## Assessment Findings

<!-- Complete one block per finding. Copy and paste for multiple findings.
     Findings here are misconfigurations, gaps, or risks — not exploits. -->

### Finding-01 — [Finding Title]

| Field | Detail |
|---|---|
| Category | e.g. IAM Misconfiguration / Insecure Default / Missing Control / Excessive Permission |
| Severity | Critical / High / Medium / Low / Informational |
| Affected Component | e.g. S3 Bucket Policy / IAM Role Trust / EC2 Security Group |
| Framework Reference | e.g. CIS AWS 1.4 / NIST AC-6 / AWS Well-Architected Security Pillar |
| Status | Open / Accepted Risk / Remediated |

**Description:**
<!-- What is the misconfiguration or gap? Explain it clearly. -->

**Evidence:**
<!-- What did you observe that confirmed this finding?
     Include config output, policy JSON, command output, or screenshots. -->
```
[Paste relevant config, policy, or command output here]
```

> Screenshot: `screenshots/finding01-[description].png`

**Risk:**
<!-- What could an attacker or insider do because of this finding?
     Be specific — not "this could lead to a breach." -->

**Recommendation:**
<!-- Specific, actionable fix with exact settings or commands where possible. -->

---

## Risk Assessment Matrix

| Finding | Likelihood (1–5) | Impact (1–5) | Risk Score | Priority |
|---|---|---|---|---|
| Finding-01 | | | | Immediate |
| Finding-02 | | | | High |
| Finding-03 | | | | Medium |

**Scoring Guide:**
- Likelihood: 1 = Unlikely, 3 = Possible, 5 = Very Likely
- Impact: 1 = Negligible, 3 = Significant, 5 = Severe
- Risk Score = Likelihood × Impact

---

## Threat Model

<!-- Who are the realistic threat actors for this environment?
     What are the most likely attack paths based on your findings? -->

**Threat Actors:**

| Actor | Motivation | Capability | Likelihood |
|---|---|---|---|
| External Attacker | Data theft | Medium | High |
| Malicious Insider | Sabotage | High | Low |
| Accidental Insider | Misconfiguration | Low | High |

**Realistic Attack Path:**
```
Threat Actor → Entry Point → [Finding ID] → Impact
Example:
External Actor → Public S3 Bucket (Finding-01) → Data Exfiltration → Data Breach
```

> Threat model diagram: `diagrams/threat-model.png`

---

## Framework / Compliance Mapping

<!-- Map your findings to the relevant framework controls.
     Only include the framework specified in the task. -->

| Control ID | Control Name | Status | Finding Reference | Gap Description |
|---|---|---|---|---|
| | | Pass / Fail / Partial | | |
| | | | | |

> Framework used: [CIS AWS Foundations / NIST CSF / ISO 27001 / AWS Well-Architected]

---

## Remediation Roadmap

| Priority | Finding | Recommended Action | Effort | Impact if Not Fixed |
|---|---|---|---|---|
| 1 — Immediate | Finding-01 | | Low / Medium / High | |
| 2 — This Week | Finding-02 | | | |
| 3 — This Month | Finding-03 | | | |

---

## Tools & Resources Used

| Tool / Resource | Purpose |
|---|---|
| AWS CLI | Enumerate IAM policies and S3 configurations |
| ScoutSuite / Prowler | Automated cloud security posture assessment |
| | |

---

## Key Lessons
<!-- Answer these three questions specifically — not a general summary: -->

**What I found that the automated tools missed:**

**What a senior cloud/security architect would do differently:**

**What I would monitor or re-check if this were a real production environment:**

---

## Loom Walkthrough
<!-- MANDATORY for Portfolio Grade and Hall of Fame review requests.
     Show the actual environment on screen. Walk through your top 3 findings.
     Explain why each finding matters and what the fix is. -->

[▶ Watch assessment walkthrough](https://loom.com/share/REPLACE-WITH-YOUR-LINK)

> Loom must cover: (1) environment overview, (2) top 3 findings with evidence,
> (3) remediation walkthrough. Minimum: 10 minutes. Maximum: 25 minutes.

---

## References

- [CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)
- [AWS Security Best Practices](https://docs.aws.amazon.com/security/)
- [MITRE ATT&CK Cloud Matrix](https://attack.mitre.org/matrices/enterprise/cloud/)
- [Add any resources you used]

---

## Submission Checklist

- [ ] Architecture diagram included in diagrams/ folder
- [ ] All findings include framework reference (CIS / NIST / AWS)
- [ ] Evidence provided for every finding (config output or screenshot)
- [ ] Risk matrix completed with scored priorities
- [ ] Remediation is specific with exact settings or commands
- [ ] Loom walkthrough recorded and linked
- [ ] Submitted on TMS with GitHub link + Loom link
