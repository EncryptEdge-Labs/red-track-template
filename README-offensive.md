# [TRACK-CODE] — Task [NN]: [Task Title]

> **Intern:** [Full Name] | **Track:** [Track Name] | **Cohort:** [N] | **Date:** YYYY-MM-DD
> **Difficulty:** [Beginner / Intermediate / Advanced] | **Duration:** [X Hours] | **Status:** [Complete / Partial]

---

## Executive Summary
<!-- 3–5 sentences written for a non-technical reader.
     What was tested? What was found? What is the business risk?
     Example: "A security assessment of [target] was conducted to identify exploitable weaknesses.
     Two critical vulnerabilities were discovered that could allow an attacker to gain full system
     access without authentication. Immediate remediation is recommended." -->

---

## Scope & Rules of Engagement

| Item | Detail |
|---|---|
| Target | |
| IP / URL / System | |
| Testing Type | [Black Box / Grey Box / White Box] |
| Authorized By | EncryptEdge Labs Lab Environment |
| Tools Permitted | |
| Out of Scope | |
| Lab Platform | [TryHackMe / HackTheBox / DVWA / Custom] |

---

## Environment Setup
<!-- Step-by-step: how did you set up your environment to complete this task?
     Include: OS, tools installed, VPN/lab connection, target configuration.
     Another intern must be able to reproduce your exact setup from these steps. -->

**Step 1:**
**Step 2:**
**Step 3:**

---

## Methodology
<!-- Which phases did this task cover? Tick all that apply and describe what you did in each. -->

- [ ] **Reconnaissance** — Passive and/or active information gathering
- [ ] **Enumeration** — Port scanning, service fingerprinting, directory busting
- [ ] **Vulnerability Identification** — Manual analysis and/or automated scanning
- [ ] **Exploitation** — Controlled, authorized exploitation of identified weaknesses
- [ ] **Post-Exploitation** — Privilege escalation, lateral movement, persistence
- [ ] **Credential Analysis** — Password cracking, hash extraction, credential abuse
- [ ] **Threat Modeling** — Attack surface mapping, MITRE ATT&CK alignment

**Methodology Notes:**
<!-- Describe your actual process — not textbook steps. What did you do first? Why?
     What decisions did you make and what drove them? -->

---

## Attack Surface Map

| Asset | Type | Port/Protocol | Risk Level | Notes |
|---|---|---|---|---|
| | | | | |
| | | | | |

<!-- Add a diagram if the attack surface is complex. Save as diagrams/attack-surface.png -->

---

## Findings Summary

| ID | Title | Severity | CVSS Score | OWASP / CWE | Status |
|---|---|---|---|---|---|
| F-01 | | Critical | | | Open |
| F-02 | | High | | | Open |
| F-03 | | Medium | | | Open |

> **Severity Count:** Critical: __ | High: __ | Medium: __ | Low: __ | Informational: __

---

## Finding Details
<!-- Repeat this block for each finding. Copy and paste. -->

### F-01 — [Finding Title]

| Field | Detail |
|---|---|
| Severity | Critical / High / Medium / Low |
| CVSS Score | |
| CVSS Vector | AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H |
| OWASP Category | e.g. A01:2021 - Broken Access Control |
| CWE Reference | e.g. CWE-89 |
| Affected Component | |
| Affected Endpoint/File | |

**Description:**
<!-- What is this vulnerability? Explain it simply. -->

**Technical Details:**
<!-- How does it work technically? What is the root cause? -->

**Proof of Concept:**
<!-- Step-by-step reproduction. A reviewer must be able to reproduce this exactly.
     Include commands, payloads, parameters used. -->
```
[commands / payloads used]
```

**Evidence:**
<!-- Reference your screenshots folder -->
> Screenshot: `screenshots/f01-[description].png`

**Impact:**
<!-- What can an attacker actually do with this? Be specific. -->

**Likelihood:**
<!-- How easy is this to exploit? Is it exposed to the internet? Does it require authentication? -->

**Risk Rating:** [Critical / High / Medium / Low]
<!-- Justify: why this severity and not higher or lower? -->

**Remediation:**
<!-- Specific, actionable fix. Not "update your software." Tell them exactly what to change. -->

---

## Threat Model

<!-- What is the most realistic attack path an adversary would take against this target?
     Map at least one complete attack chain using the format below. -->

**Attack Chain:**
```
Initial Access → [technique] → [MITRE TID]
Execution     → [technique] → [MITRE TID]
Privilege Esc → [technique] → [MITRE TID]
Impact        → [technique] → [MITRE TID]
```

> Diagram: `diagrams/threat-model.png` (required for Portfolio Grade and above)

---

## Risk Matrix

| Finding | Likelihood (1-5) | Impact (1-5) | Risk Score | Priority |
|---|---|---|---|---|
| F-01 | | | | Immediate |
| F-02 | | | | High |
| F-03 | | | | Medium |

---

## Remediation Roadmap

| Priority | Finding | Recommended Fix | Effort | Owner |
|---|---|---|---|---|
| 1 — Immediate | F-01 | | Low / Medium / High | Dev / SecOps |
| 2 — This Week | F-02 | | | |
| 3 — This Month | F-03 | | | |

---

## Tools Used

| Tool | Version | Purpose |
|---|---|---|
| | | |
| | | |

---

## Key Lessons
<!-- This is not a summary. Answer these three questions specifically:
     1. What did you discover that surprised you or was not in the task instructions?
     2. What would a professional consultant do differently than you did?
     3. What would you look for next if you had more time? -->

**Surprise finding:**

**What a professional would do differently:**

**What I would investigate next:**

---

## Loom Walkthrough
<!-- MANDATORY for Portfolio Grade and Hall of Fame review requests.
     Record yourself: demo the exploit live, explain your severity rating, walk through remediation. -->

[▶ Watch verification walkthrough](https://loom.com/share/REPLACE-WITH-YOUR-LINK)

> Loom must cover: (1) live exploit demo, (2) CVSS justification, (3) remediation explanation.
> Minimum: 10 minutes. Maximum: 25 minutes.

---

## References

- [OWASP](https://owasp.org)
- [MITRE ATT&CK](https://attack.mitre.org)
- [NVD CVE](https://nvd.nist.gov)
- [Add any resources you used]

---

## Submission Checklist

- [ ] All finding blocks completed with CVSS + OWASP
- [ ] Screenshots annotated (red boxes, arrows, labels)
- [ ] At least one diagram included
- [ ] Loom walkthrough recorded and linked
- [ ] Remediation is specific and actionable (not generic)
- [ ] Executive summary uses non-technical language
- [ ] Submitted on TMS with GitHub link + Loom link
