# [TRACK-CODE] — Task [NN]: [Task Title]

> **Intern:** [Full Name] | **Track:** [Track Name] | **Cohort:** [N] | **Date:** YYYY-MM-DD
> **Difficulty:** [Beginner / Intermediate / Advanced] | **Duration:** [X Hours] | **Status:** [Complete / Partial]

---

## Investigation Summary
<!-- 3–5 sentences for a non-technical reader or senior analyst.
     What was investigated? What was found? What decision was made?
     Example: "An authentication alert triggered by a suspected brute-force attack was investigated.
     Analysis confirmed malicious activity originating from an external IP across three user accounts.
     Two accounts were compromised. Escalation to Tier-2 is recommended with immediate password reset." -->

---

## Investigation Scope

| Item | Detail |
|---|---|
| Alert / Task Type | [Alert Triage / Log Analysis / Traffic Analysis / Incident Simulation] |
| Data Sources Used | e.g. Windows Event Logs, Syslog, SIEM, PCAP, EDR Alerts |
| Time Range Analysed | YYYY-MM-DD HH:MM to YYYY-MM-DD HH:MM |
| Systems / Accounts in Scope | |
| Lab Platform | [Splunk / ELK / LimaCharlie / Wazuh / TryHackMe / HackTheBox] |
| Task Objective | [Copy from task description — one sentence] |

---

## Environment Setup
<!-- How did you set up or access the environment for this task?
     Include: SIEM platform, log source, dataset loaded, tools used.
     Another intern must be able to reproduce your setup from these steps. -->

**Step 1:**
**Step 2:**
**Step 3:**

---

## Evidence Sources

| Source | Type | What It Provided |
|---|---|---|
| | Windows Event Log | Authentication events |
| | Firewall Log | Inbound/outbound traffic |
| | EDR Alert | Process execution on endpoint |
| | SIEM Dashboard | Correlated alert view |
| | PCAP File | Raw network traffic |

<!-- Add or remove rows based on what you actually used. Do not include sources you did not use. -->

---

## Investigation Methodology

<!-- Which of these did this task require? Tick all that apply. -->

- [ ] **Alert Triage** — Reviewing alert queue, assessing priority and context
- [ ] **Log Analysis** — Querying and interpreting raw log data
- [ ] **Traffic Analysis** — Examining network flows, sessions, or PCAP data
- [ ] **Timeline Reconstruction** — Building chronological sequence of events
- [ ] **IOC Validation** — Checking indicators against threat intelligence
- [ ] **MITRE ATT&CK Mapping** — Linking observed behavior to ATT&CK techniques
- [ ] **False Positive Analysis** — Determining if alert was benign or malicious
- [ ] **Escalation Decision** — Deciding whether to close, monitor, or escalate

**Approach:**
<!-- Describe your actual investigative process. What did you look at first? Why?
     What hypothesis did you form and how did you test it? -->

---

## Event Timeline

| Timestamp (UTC) | Event | Source | Significance |
|---|---|---|---|
| YYYY-MM-DD HH:MM:SS | | | |
| YYYY-MM-DD HH:MM:SS | | | |
| YYYY-MM-DD HH:MM:SS | | | |

<!-- Build this from actual log/alert data. Do not approximate timestamps.
     Significance = why does this event matter to the investigation? -->

---

## Alert Analysis

<!-- Complete one block per alert or finding. Copy and paste for multiple alerts. -->

### Alert-01 — [Alert Name / Rule Name]

| Field | Detail |
|---|---|
| Alert ID / Rule | |
| Severity | Critical / High / Medium / Low / Informational |
| Source System | |
| Triggered By | |
| Initial Classification | True Positive / False Positive / Benign True Positive |

**Alert Context:**
<!-- What was happening when this alert fired? What is the normal baseline?
     Why is this alert flagged as suspicious rather than normal activity? -->

**Evidence Supporting Classification:**
<!-- What specific log entries, traffic patterns, or process behaviors support your conclusion?
     Quote exact log fields where possible. -->

```
[Paste relevant log entry, query result, or event data here]
```

> Screenshot: `screenshots/alert01-[description].png`

**Analyst Decision:** [Escalate / Monitor / Close — False Positive / Close — Resolved]

**Justification:**
<!-- Why did you make this decision? What evidence drove it?
     What would change your decision if you had more information? -->

---

## MITRE ATT&CK Mapping

| Tactic | Technique | Technique ID | Observed Behavior | Evidence |
|---|---|---|---|---|
| e.g. Initial Access | Phishing | T1566 | | |
| e.g. Credential Access | Brute Force | T1110 | | |
| e.g. Lateral Movement | Pass the Hash | T1550.002 | | |

> Reference: [MITRE ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/)
> Save navigator export as: `appendix/mitre-navigator-export.json`

---

## Indicators of Compromise (IOCs)

| Type | Value | Confidence | Source |
|---|---|---|---|
| IP Address | | High / Medium / Low | |
| Domain | | | |
| File Hash (MD5/SHA256) | | | |
| Username | | | |
| User-Agent | | | |

<!-- Only include IOCs you actually identified during this investigation.
     Leave table empty and note "No IOCs identified" if none found. -->

---

## Visibility Gaps & Limitations
<!-- What data was missing that would have helped this investigation?
     What log sources were not available? What would you add to improve detection? -->

**What was missing:**

**How it affected the investigation:**

**What I would add to improve detection:**

---

## Escalation Recommendation

**Decision:** [Escalate to Tier-2 / Monitor and Watch / Close — Resolved / Close — False Positive]

**Severity Rating:** [Critical / High / Medium / Low / Informational]

**Reason:**
<!-- Write 3–5 sentences justifying your escalation decision as if handing this to a senior analyst. -->

**Immediate Actions Required:**
<!-- What should happen in the next hour? Next 24 hours? -->

- [ ] Immediate (0–1 hour):
- [ ] Short-term (1–24 hours):
- [ ] Follow-up (24–72 hours):

---

## Analyst Notes
<!-- Raw working notes. What queries did you run? What dead ends did you hit?
     What did you rule out and why? This section demonstrates your analytical thinking. -->

**Queries run:**
```
[Paste SIEM/log queries you used]
```

**Dead ends:**

**What I ruled out and why:**

---

## Key Lessons
<!-- Answer these three questions specifically — not a summary of what you did: -->

**What surprised me about this investigation:**

**What a senior analyst would do differently:**

**What I would monitor going forward if this were a real environment:**

---

## Loom Walkthrough
<!-- MANDATORY for Portfolio Grade and Hall of Fame review requests.
     Record yourself: walk through your timeline, explain your MITRE mapping,
     justify your escalation decision. Show the actual SIEM/log data on screen. -->

[▶ Watch investigation walkthrough](https://loom.com/share/REPLACE-WITH-YOUR-LINK)

> Loom must cover: (1) timeline walkthrough, (2) MITRE ATT&CK mapping explanation,
> (3) escalation decision justification. Minimum: 10 minutes. Maximum: 25 minutes.

---

## References

- [MITRE ATT&CK](https://attack.mitre.org)
- [Sigma Rules](https://github.com/SigmaHQ/sigma)
- [NIST IR Guide](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)
- [Add any resources you used]

---

## Submission Checklist

- [ ] Event timeline built from actual log timestamps (not approximated)
- [ ] MITRE ATT&CK mapping completed with Technique IDs
- [ ] All screenshots annotated and referenced in the report
- [ ] Escalation decision clearly justified
- [ ] Analyst notes section completed (queries + dead ends)
- [ ] Loom walkthrough recorded and linked
- [ ] Submitted on TMS with GitHub link + Loom link
