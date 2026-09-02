# Nicholas Quist

**Machine learning applied to security problems** — and evaluating the models other people build.

M.S. Data Science & Artificial Intelligence at UNC Wilmington, following a B.S. in Cybersecurity there.

I came into ML through security, and the overlap is the part I care about: getting messy real-world security data into a shape a model can actually learn from, and being honest about what the results do and don't prove.

[LinkedIn](https://www.linkedin.com/in/nicholasquist/) · [LetsDefend](https://app.letsdefend.io/user/quist) · [Hack The Box](https://profile.hackthebox.com/profile/019c498b-e549-7061-b8cd-6586b4980ed0)

---

## Projects

| Project | What it is |
|---|---|
| [**soc-analyst-simulator**](https://github.com/nicky-quist/soc-analyst-simulator) | A working Tier-1 analyst console, built to practise the whole shift rather than quiz you on it: you investigate by typing your own searches against **18 simulated data sources**, pull indicators out of the evidence yourself, and take response actions that carry consequences — **53 of them, 20 of which are mistakes** a CISO, IR lead, and employment lawyer react to. Seven scenarios, 150 events, **52 tests** over the scoring and query engines. [Live demo](https://nicky-quist.github.io/soc-analyst-simulator/) |
| [**attack-path-modeler**](https://github.com/nicky-quist/attack-path-modeler) | Builds a segmentation-aware attack graph from Nessus or bare CVE IDs, then trains a **3-layer PyTorch Geometric GCN** to predict which edges lie on an optimal route to a crown-jewel asset. Exploitability comes from **EPSS + CISA KEV**, not CVSS — edges are weighted `-log(P(exploit))`, so Dijkstra returns the *most probable* attack chain and its cost converts back to a success probability. Benchmarked against three baselines over 5 independent networks (**F1 0.911 ± 0.151** vs 0.768 with no message passing). 28 tests, including regressions for the label-leakage bug I found in my own earlier version. |
| [**llm-cybersecurity-benchmark**](https://github.com/nicky-quist/llm-cybersecurity-benchmark) | Head-to-head evaluation of **11 models from Google, OpenAI and Anthropic** across **28 blind pairwise comparisons** (27 of 28 cross-vendor) — threat reasoning, detection engineering, hallucination traps. Bradley-Terry strengths with bootstrap CIs and per-model Wilson intervals: GPT-4o (0-for-6) is the only model that separates from parity, and the vendor-level split is not significant (χ² p=0.47). [Live dashboard](https://nicky-quist.github.io/llm-cybersecurity-benchmark/dashboard/index.html) with per-category filtering and matchup-level results. Submitted to the Codex Creator Challenge 2026. |
| [**soc-triage-tool**](https://github.com/nicky-quist/soc-triage-tool) | React app with a deterministic, fully offline rule engine — no API calls. Detects log format across 6 types (syslog, Windows Event, Suricata, Zeek, CEF, JSON), maps to MITRE ATT&CK, extracts IOCs, scores severity, recommends a next action. [Live demo](https://nicky-quist.github.io/soc-triage-tool/) |
| [**splunk-detections**](https://github.com/nicky-quist/splunk-detections) | Three detections validated against live Sysmon/Windows Security telemetry: multi-signal suspicious PowerShell, local-admin creation correlated with first logon, and password spray on Event ID 4625. Each with data requirements, investigation pivots, and false-positive tuning notes. |
| [**windows-event-labs**](https://github.com/nicky-quist/windows-event-labs) | Labs on the Windows Security and Sysmon event IDs that carry real signal, with process, network, and logon correlation worked end to end. |
| [**rmf-security-assessment-sample**](https://github.com/nicky-quist/rmf-security-assessment-sample) | A full NIST RMF assessment lifecycle for a fictional case-management system — categorization through ATO recommendation. |

---

## What I'm good at

**Graph ML on messy data** — modeling networks as graphs and learning over their structure. Edge classification, centrality analysis, and feature design that starts from what a scanner actually outputs rather than what would be convenient.

**Evaluating models properly** — benchmarks that separate models instead of flattering them: stratified prompt sets, head-to-head scoring, results you can drill into by category. Also what I do professionally.

**Domain grounding** — detection engineering, log analysis, risk assessment. A summer triaging 10–30 alerts a day and writing Suricata rules from live PCAP is why I know what this data looks like before it's been cleaned up for a paper.

**Auditing my own results** — the attack-path GNN used to report 100% precision and recall. I went back and found why: the training label was `target.max_cvss > 8.5` while `max_cvss` was also an input feature, so a one-line threshold scored 100% too and the model had learned nothing. I rewrote the target as a graph-structural one, added the baselines that would have caught it, and the honest number is F1 0.911 ± 0.151 against 0.768 for a no-graph model. A result nobody can reproduce a baseline for isn't a result.

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
