# Nicholas Quist — SOC / Blue Team

I build practical detections, investigate alerts end-to-end, and document my work like a real SOC: **triage → pivot → timeline → IOCs → detection → tuning**.

---

## What I work on
- **Splunk SPL detections + alert tuning**
- **Network investigations** (PCAP → IOCs → SIEM pivots)
- **Suricata rules + validation** (test PCAPs + false-positive notes)
- **Windows Event Logs / Sysmon** (process, auth, persistence tracking)
- (Optional) **OT/ICS monitoring** (protocol behavior + detection ideas)

---

## How I work (SOC workflow)
1) Validate the alert (is it real? what’s the evidence?)  
2) Pivot across host/user/network indicators  
3) Build a timeline + capture IOCs  
4) Contain/escalate with clear justification  
5) Write or tune detections so it’s easier next time  

---

## Pinned Projects (start here)
- 🔎 **splunk-detections** — SPL detections with MITRE mapping + tuning notes  
- 🧪 **pcap-investigations** — case studies with timelines + IOCs + detection ideas  
- 🛡️ **suricata-rules-lab** — Suricata rules + test PCAP validation + FP tuning  
- 📋 **soc-triage-playbooks** — alert triage checklists + escalation thresholds  
- 🪟 **windows-event-labs** — Windows/Sysmon telemetry notes + hunting pivots  
- 🛰️ **nmap-log-analysis** — recon detection writeup using Nmap/Wireshark/Suricata/Splunk  

---

## Detection pack roadmap (in progress)
- Suspicious PowerShell (encoded/obfuscated + download cradle patterns)
- Local admin creation + first logon correlation
- Service creation persistence (user-writable paths, uncommon binaries)
- Multiple failed logons → success (brute force / password spray indicators)
- Suspicious outbound DNS patterns (rare domains, high NXDOMAIN)

---

## Lab environment & data sources
- Windows telemetry: Security logs + (optional) Sysmon
- Network telemetry: PCAPs, Suricata alerts, DNS/HTTP metadata
- Output: Investigation notes, timelines, IOCs, and detections that can be reproduced

---

## Skills
Splunk SPL, Windows Event Logs, Wireshark, Suricata, Nmap/Nessus basics, MITRE ATT&CK mapping
