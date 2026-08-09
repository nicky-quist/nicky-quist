# Nicholas Quist

SOC / Blue Team — Splunk SPL detections, PCAP/Suricata investigations, IR triage.
Student at UNC Wilmington.

I build practical detections, investigate alerts end-to-end, and document the work like a real SOC would: **triage → pivot → timeline → IOCs → detection → tuning.**

[LinkedIn](https://www.linkedin.com/in/nicholasquist/) · [LetsDefend](https://app.letsdefend.io/user/quist) · [Hack The Box](https://profile.hackthebox.com/profile/019c498b-e549-7061-b8cd-6586b4980ed0)

---

## Projects

| Project | What it is |
|---|---|
| [**soc-triage-tool**](https://github.com/nicky-quist/soc-triage-tool) | React app that triages a pasted alert (syslog, Windows Event, Suricata, Zeek, CEF) — detects the log format, scores severity, and maps it to MITRE ATT&CK. [Live demo](https://nicky-quist.github.io/soc-triage-tool/) |
| [**splunk-detections**](https://github.com/nicky-quist/splunk-detections) | SPL detections with data requirements, investigation pivots, MITRE mapping, and false-positive tuning notes for each one |
| [**llm-cybersecurity-benchmark**](https://github.com/nicky-quist/llm-cybersecurity-benchmark) | Head-to-head benchmark of LLMs on SOC analysis tasks — detection engineering, threat reasoning, IR scenarios — with an interactive results dashboard |
| [**attack-path-modeler**](https://github.com/nicky-quist/attack-path-modeler) | Parses Nessus scan data into an attack graph, ranks lateral-movement paths by exploit difficulty, and visualizes it with matplotlib + an interactive D3 dashboard |
| [**rmf-security-assessment-sample**](https://github.com/nicky-quist/rmf-security-assessment-sample) | A full NIST RMF assessment lifecycle worked end-to-end for a fictional case-management system — categorization through ATO recommendation |
| [**windows-event-labs**](https://github.com/nicky-quist/windows-event-labs) | Hands-on labs on high-signal Windows Security + Sysmon event IDs, with process/network correlation writeups |
| [**pcap-investigations**](https://github.com/nicky-quist/pcap-investigations) | Network investigation case studies — PCAP → IOCs → timeline → SIEM pivots |
| [**soc-triage-playbooks**](https://github.com/nicky-quist/soc-triage-playbooks) | Alert triage checklists and escalation thresholds by alert type |
| [**nmap-log-analysis**](https://github.com/nicky-quist/nmap-log-analysis) | Recon-detection writeup correlating Nmap scan activity across Wireshark, Suricata, and Splunk |

---

## How I work an alert
1. **Validate** — is it real, what's the evidence
2. **Pivot** — across host, user, and network indicators
3. **Timeline** — reconstruct sequence, capture IOCs
4. **Contain / escalate** — with justification, not guesswork
5. **Tune** — turn the investigation into a detection or a fix, so it's faster next time

## Skills
Splunk SPL · Windows Event Logs & Sysmon · Wireshark · Suricata · Nmap / Nessus · MITRE ATT&CK mapping

## Currently building
Detection pack: encoded/obfuscated PowerShell, local admin creation + first-logon correlation, service-creation persistence, password-spray indicators, and anomalous outbound DNS.
