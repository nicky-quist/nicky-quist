# Nicholas Quist — SOC / Blue Team

I build practical detections, investigate alerts end-to-end, and document each case using a repeatable SOC workflow:
**triage → pivot → timeline → IOCs → detection → tuning**.

---

## What you'll find here
- **Splunk detections + alert tuning**
- **Network investigations** (PCAP analysis, IOC extraction, SIEM pivots)
- **Suricata rules + validation** (test PCAPs + false-positive tracking)
- **Windows Security Logs / Sysmon analysis**
- **OT/ICS monitoring notes** (protocol behavior + detection ideas)

---

## SOC workflow I use
1. Validate the alert (scope, confidence, and evidence).
2. Pivot across host, user, and network indicators.
3. Build a timeline and capture IOCs.
4. Contain/escalate with clear justification.
5. Write or tune detections to reduce repeat effort.

---

## Pinned projects (start here)
- **splunk-detections** — SPL detections with MITRE ATT&CK mapping + tuning notes.
- **pcap-investigations** — Case studies with timelines, IOCs, and follow-on detections.
- **suricata-rules-lab** — Suricata signatures with test PCAP validation and FP tuning.
- **soc-triage-playbooks** — Triage checklists and escalation thresholds.
- **windows-event-labs** — Windows/Sysmon telemetry labs and hunting pivots.
- **nmap-log-analysis** — Reconnaissance detection write-up using Nmap, Wireshark, Suricata, and Splunk.

---

## Detection roadmap
- Suspicious PowerShell (encoded/obfuscated commands + download cradle behavior)
- Local admin creation correlated with first successful logon
- Service-creation persistence (user-writable paths, uncommon binaries)
- Multiple failed logons followed by success (spray/brute-force indicators)
- Suspicious outbound DNS behavior (rare domains, high NXDOMAIN)

---

## Lab environment & data sources
- **Host telemetry:** Windows Security logs + optional Sysmon
- **Network telemetry:** PCAPs, Suricata alerts, DNS/HTTP metadata
- **Deliverables:** investigation notes, timelines, IOC sets, and reproducible detections

---

## Core skills
Splunk SPL, Windows Event Logs, Wireshark, Suricata, Nmap/Nessus fundamentals, MITRE ATT&CK mapping
