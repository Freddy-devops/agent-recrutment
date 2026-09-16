# Autonomous AI Recruitment & Candidate Screening Suite (Code Caméléon)

An enterprise-ready, compliant multi-agent recruitment suite engineered with CrewAI. It automates resume parsing, candidate qualification scoring, and regional regulatory compliance (EU AI Act, GDPR, EEOC).

## 🚀 Key Features

* **🛡️ Resume Prompt Injection Firewall**: Input encapsulation (`<candidature_entrante>`) to protect against candidate attempts to hijack screening prompts or force evaluation outcomes.
* **🎯 3-Tier Qualification Engine**: Structured evaluation assigning strict candidate outcomes (**VALIDE**, **INCOMPLET**, **REJETÉ**) based on job-matching algorithms.
* **🌍 "Code Caméléon" HR Compliance**: Dynamic jurisdiction detection (ISO country codes) injecting legally required disclaimers (EU AI Act transparency rules, US EEOC compliance, regional retention policies).
* **🔑 Multi-Tenant Candidate Data Purge**: Surgical GDPR Kill Switch (`kill_switch_rgpd_rh`) for instant Right-to-be-Forgotten compliance per candidate without compromising database integrity.
* **⚡ Async Pipeline**: Non-blocking asynchronous execution (`kickoff_async`) designed for cloud integrations (AWS SES, Webhooks, ATS platforms).

## 🛠️ Tech Stack

* **Multi-Agent Engine**: [CrewAI](https://github.com/joaomdmoura/crewai)
* **LLM Orchestration**: Gemini 3.5 Flash-lite (via `litellm`)
* **Language**: Python 3.10+
* **Environment Control**: `python-dotenv`, `nest_asyncio`

## 📂 Repository Structure

```text
recruitment-ai-agent/
├── .gitignore          # Excluded local environments and keys
├── requirements.txt    # Production dependencies
├── README.md           # Documentation
├── SECURITY.md         # Security & HR compliance standards
└── main.py             # Agent definitions, tasks, and execution flow