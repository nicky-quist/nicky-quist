# Nicholas Quist

**Machine learning applied to security problems** — and evaluating the models other people build.

M.S. Data Science & Artificial Intelligence at UNC Wilmington (Fall 2026 – December 2027), following a B.S. in Cybersecurity there. Currently an AI Model Evaluation Contractor at **Handshake AI**, grading frontier model outputs for technical accuracy, reasoning quality, and hallucination risk.

I came into ML through security, and the overlap is the part I care about: getting messy real-world security data into a shape a model can actually learn from, and being honest about what the results do and don't prove.

[LinkedIn](https://www.linkedin.com/in/nicholasquist/) · [LetsDefend](https://app.letsdefend.io/user/quist) · [Hack The Box](https://profile.hackthebox.com/profile/019c498b-e549-7061-b8cd-6586b4980ed0)

---

## Projects

| Project | What it is |
|---|---|
| [**soc-analyst-simulator**](https://github.com/nicky-quist/soc-analyst-simulator) | A working Tier-1 analyst console, built to practise the whole shift rather than quiz you on it: you investigate by typing your own searches against **18 simulated data sources**, pull indicators out of the evidence yourself, and take response actions that carry consequences — **53 of them, 20 of which are mistakes** a CISO, IR lead, and employment lawyer react to. Seven scenarios, 150 events, **52 tests** over the scoring and query engines. [Live demo](https://nicky-quist.github.io/soc-analyst-simulator/) |
| [**attack-path-modeler**](https://github.com/nicky-quist/attack-path-modeler) | Turns Nessus scan data into a directed attack graph, then trains a **PyTorch Geometric GCN** to predict which lateral-movement edges are high risk. Two GCNConv layers with a skip connection, class-weighted training on an 80/20 edge split. Ranks paths with Dijkstra weighted by exploit ease, finds choke points via betweenness centrality, pulls live CVSS from the NVD API. Interactive D3 dashboard. |
| [**llm-cybersecurity-benchmark**](https://github.com/nicky-quist/llm-cybersecurity-benchmark) | Head-to-head evaluation of **8 Google and OpenAI models** across **20 security prompts** in 20 categories — threat reasoning, malware analysis, detection engineering, hallucination traps. [Live dashboard](https://nicky-quist.github.io/llm-cybersecurity-benchmark/dashboard/index.html) with per-category filtering and matchup-level results. Submitted to the Codex Creator Challenge 2026. |
| [**soc-triage-tool**](https://github.com/nicky-quist/soc-triage-tool) | React app with a deterministic, fully offline rule engine — no API calls. Detects log format across 6 types (syslog, Windows Event, Suricata, Zeek, CEF, JSON), maps to MITRE ATT&CK, extracts IOCs, scores severity, recommends a next action. [Live demo](https://nicky-quist.github.io/soc-triage-tool/) |
| [**splunk-detections**](https://github.com/nicky-quist/splunk-detections) | Three detections validated against live Sysmon/Windows Security telemetry: multi-signal suspicious PowerShell, local-admin creation correlated with first logon, and password spray on Event ID 4625. Each with data requirements, investigation pivots, and false-positive tuning notes. |
| [**windows-event-labs**](https://github.com/nicky-quist/windows-event-labs) | Labs on the Windows Security and Sysmon event IDs that carry real signal, with process, network, and logon correlation worked end to end. |
| [**rmf-security-assessment-sample**](https://github.com/nicky-quist/rmf-security-assessment-sample) | A full NIST RMF assessment lifecycle for a fictional case-management system — categorization through ATO recommendation. |

---

## What I'm good at

**Graph ML on messy data** — modeling networks as graphs and learning over their structure. Edge classification, centrality analysis, and feature design that starts from what a scanner actually outputs rather than what would be convenient.

**Evaluating models properly** — benchmarks that separate models instead of flattering them: stratified prompt sets, head-to-head scoring, results you can drill into by category. Also what I do professionally.

**Domain grounding** — detection engineering, log analysis, risk assessment. A summer triaging 10–30 alerts a day and writing Suricata rules from live PCAP is why I know what this data looks like before it's been cleaned up for a paper.

**Stating what a result doesn't prove** — the attack-path GNN hits 100% precision/recall on held-out synthetic edges. The writeup says plainly that it hasn't been validated against real scan data, and that real data will be noisier. Numbers without that caveat aren't worth much.

---

## Skills

**ML & AI** — PyTorch · PyTorch Geometric · Graph Neural Networks · LLM evaluation & benchmark design · feature engineering · Claude API · Jupyter

**Programming & Data** — Python · PowerShell · JavaScript/React · NetworkX · graph algorithms · D3.js · matplotlib · Git

**Detection & SIEM** — Splunk SPL · detection engineering · Suricata · Sigma · Sysmon · Windows Event Logs · threat hunting

**Security Tooling & Frameworks** — Nessus · Nmap · Wireshark · VirusTotal · Microsoft Defender · MITRE ATT&CK · NIST RMF / 800-53 / CSF · Linux (Ubuntu/Kali)

---

## Credentials

CompTIA Security+ (SY0-701), valid through May 2028 · CISA ICS Cybersecurity (ICS-300) · Linear Algebra for Machine Learning & Data Science (DeepLearning.AI)

U.S. Citizen · eligible for security clearance

## Currently building

Training the attack-path GNN on real heterogeneous scan data instead of synthetic graphs, and mapping MITRE ATT&CK techniques per CVE.
