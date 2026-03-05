# 🛡️ Cybersecurity from Scratch — Final Course Project

> **Course:** [Кібербезпека з нуля — RobotDreams](https://robotdreams.cc/uk/course/2416-kiberbezpeka-z-nulya#about)  
> **Student:** Bohdan Lutsyk

---

## 📋 Table of Contents

- [Part 1 — Red Team for AI](#part-1----red-team-for-ai)
- [Part 2 — App Security Analysis](#part-2----app-security-analysis-vulnshop-11)

---

## Part 1 — 🤖 Red Team for AI

### Description

Security vulnerability testing on Large Language Models (LLMs) to gain practical experience in AI Red Teaming. Simulating adversarial attacks to identify weaknesses in how models handle malicious prompts.

### Key Objectives

| # | Objective | Details |
|---|-----------|---------|
| 1 | **Environment Setup** | Deploy a local testing environment using Ollama + NVIDIA Garak |
| 2 | **Vulnerability Assessment** | Execute attack probes against `mistral:latest` and `phi3:mini` |
| 3 | **Analysis & Reporting** | Analyze hitlogs and HTML reports to determine model failure rates |
| 4 | **Documentation** | Formal report with Executive Summary, PoC, and Remediation |

### Attack Vectors Tested

- 🔓 **Jailbreaks (DAN)** — Bypassing the model's safety guardrails
- 🔢 **Encoding Attacks** — Using Base64, ROT13, or Hex to hide malicious intent
- 💉 **Prompt Injection** — Manipulating model output through injected instructions

### Materials

<details>
<summary>📄 Reports & Documentation</summary>

1. `Control_Questions.pdf` — Additional answers for control questions
2. `Lutsyk_RedTeam_AI_Report.pdf` — Report for **mistral** model scan
3. `Lutsyk_RedTeam_AI_Report_phi3_mini.pdf` — Report for **phi3:mini** model scan

</details>

<details>
<summary>📎 Appendices — mistral:latest</summary>

**Hitlogs & HTML Reports:**
- `garak.mistral_latest_Comprehensive_test.hitlog.jsonl` / `.report.html`
- `garak.mistral_latest_Dan.hitlog.jsonl` / `.report.html`
- `garak.mistral_latest_encoding.hitlog.jsonl` / `.report.html`
- `garak.mistral_latest_promtinject.hitlog.jsonl` / `.report.html`

**Screenshots:**
- `mistral_latest_comprehensive_test.png`
- `mistral_latest_dan.png`
- `mistral_latest_encoding.png`
- `mistral_latest_promtinject.png`
- `postman_dan.png`
- `postman_promtinjection.png`

</details>

<details>
<summary>📎 Appendices — phi3:mini</summary>

**Hitlogs & HTML Reports:**
- `garak.phi3_mini_Comprehensive_test.hitlog.jsonl` / `.report.html`
- `garak.phi3_mini_Dan.hitlog.jsonl` / `.report.html`
- `garak.phi3_mini_encoding.hitlog.jsonl` / `.report.html`
- `garak.phi3_mini_promtinject.hitlog.jsonl` / `.report.html`

**Screenshots:**
- `phi3_mini_comprehensive_test.png`
- `phi3_mini_dan.png`
- `phi3_mini_encoding.png`
- `phi3_mini_promtinject.png`
- `postman_dan_phi3.png`
- `postman_promtinjection_phi3.png`

</details>

---

## Part 2 — 🕵️ App Security Analysis (vulnshop-1.1)

### Description

Vulnerability testing on a web application — demonstrating exploitation techniques and preparing a formal results report. The application was deployed in a test environment with active exploration permitted.

### Key Objectives

| # | Objective | Details |
|---|-----------|---------|
| 1 | **Reconnaissance** | Initial information gathering; locate hidden resources and service files |
| 2 | **Vulnerability Exploitation** | Demonstrate critical attack vectors (see below) |
| 3 | **Flag Capture** | Retrieve flags hidden in application directories as proof of exploitation |
| 4 | **Professional Reporting** | Detailed report with step-by-step PoC, risk assessment, and remediation |

### Attack Vectors Demonstrated

- 🔑 **Broken Access Control (IDOR)** — Bypassing restrictions to access unauthorized data
- 🗄️ **SQL Injection** — Gaining administrative access via injection attacks
- 💻 **Remote Code Execution (RCE)** — Running arbitrary commands on the server
- 🌐 **Cross-Site Scripting (XSS)** — Executing arbitrary client-side code

### Materials

<details>
<summary>📄 Reports & Documentation</summary>

1. `Lutsyk_VulnShop_Security_Report.pdf` — Full security report

</details>

<details>
<summary>📎 Appendices — Screenshots by Stage</summary>

| Stage | File |
|-------|------|
| Stage 1 — Reconnaissance | `Stage1_Reconnaissance.png` |
| Stage 2 — Hidden Directories | `Stage2_Hidden_Directories.png` |
| Stage 3 — IDOR | `Stage3_IDOR.png` |
| Stage 4 — SQL Injection | `Stage4_SQLInjection1.png` through `Stage4_SQLInjection7_2.png` (10 files) |
| Stage 5 — XSS | `Stage5_XSS1.png`, `Stage5_XSS2.png` |
| Stage 6 — RCE | `Stage6_RCE1.png` through `Stage6_RCE4.png` |

</details>
