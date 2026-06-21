[README.md](https://github.com/user-attachments/files/29181878/README.md)
# 🚗 AI Process Automation Analyzer
### Built for Mercedes-Benz — KI & Automatisierung Internship

A browser-based AI tool that analyzes any business process, scores its automation potential, generates a ready-to-use **Power Automate flow**, and creates a **presentation concept for non-technical stakeholders** — all in under 30 seconds.

> Built as a Proof-of-Concept for the Mercedes-Benz AI & Automation internship role. Demonstrates hands-on skills in generative AI, process analysis, low-code automation design, and communicating AI concepts to business audiences.

---

## ✨ What it does

Paste a business process description → the AI agent returns:

| Output | Description |
|--------|-------------|
| **Automation Score** | How automatable is this process? (0–100) |
| **ROI Score** | Estimated business value of automating it |
| **Ease of Implementation** | How complex would it be to build? |
| **Pain Point Analysis** | Key friction points identified by AI |
| **Step-by-step breakdown** | Each process step labeled: automatable / partial / manual |
| **Power Automate Flow** | Ready connector-by-connector flow design |
| **Presentation concept** | 4 talking points for non-technical stakeholders |
| **Copilot use case** | How Microsoft Copilot fits into this specific process |

---

## 🖥️ Screenshots

### 1. Input — describe any business process
```
┌─────────────────────────────────────────────────────────┐
│  ✦ KI & Automatisierung          [MB Logo]              │
│─────────────────────────────────────────────────────────│
│  API Key: [sk-ant-...]                                  │
│                                                         │
│  Process description:                                   │
│  ┌─────────────────────────────────────────────────┐   │
│  │ Every Monday, the procurement team downloads    │   │
│  │ supplier invoices from 3 email inboxes,         │   │
│  │ manually enters data into SAP...                │   │
│  └─────────────────────────────────────────────────┘   │
│                                                         │
│  Try: [Invoice approval] [Supplier onboarding]          │
│       [Quality reporting] [Meeting follow-ups]          │
│                                                         │
│  Department: [Einkauf / Procurement ▾]                  │
│  Effort/month: [15–40 hours ▾]                          │
│                                                         │
│  [    ⚡ Analyze process with AI    ]                   │
└─────────────────────────────────────────────────────────┘
```

### 2. Results — AI scores + analysis
```
┌──────────────────┬──────────────────┬──────────────────┐
│ Automation       │ ROI              │ Ease of          │
│ potential        │ potential        │ implementation   │
│                  │                  │                  │
│      87          │      91          │      74          │
│    (green)       │    (green)       │    (green)       │
│ ████████████░░ │ ██████████████░ │ ████████████░░░ │
└──────────────────┴──────────────────┴──────────────────┘
```

### 3. Process step breakdown
```
┌─────────────────────────────────────────────────────────┐
│ 🔍 Process step analysis                                │
│─────────────────────────────────────────────────────────│
│ ① Email monitoring & invoice download                   │
│   Procurement team checks 3 inboxes manually            │
│   [✓ Automatable]  [Outlook]                           │
│ ──────────────────────────────────────────              │
│ ② Data entry into SAP                                   │
│   Invoice fields copied manually into ERP               │
│   [⟳ Partial]  [SAP connector]                        │
│ ──────────────────────────────────────────              │
│ ③ Duplicate check in Excel                              │
│   Cross-references existing records manually             │
│   [✓ Automatable]  [Excel / Dataverse]                 │
│ ──────────────────────────────────────────              │
│ ④ Approval email to department heads                    │
│   Manual email drafting and follow-up                   │
│   [✓ Automatable]  [Outlook + Approvals]               │
└─────────────────────────────────────────────────────────┘
```

### 4. Power Automate flow design
```
┌─────────────────────────────────────────────────────────┐
│ ⚡ Suggested Power Automate flow                        │
│─────────────────────────────────────────────────────────│
│ 📧  When email arrives with attachment    [Outlook]     │
│                      ↓                                  │
│ 🤖  Extract invoice data with AI Builder  [AI Builder]  │
│                      ↓                                  │
│ 🔍  Check for duplicates in database      [Dataverse]   │
│                      ↓                                  │
│ ✅  Send approval request to managers     [Approvals]   │
│                      ↓                                  │
│ 📊  Update SAP & archive to SharePoint    [SAP / SPO]   │
│─────────────────────────────────────────────────────────│
│ ✅ Estimated time saved: ~24 hours/month                │
└─────────────────────────────────────────────────────────┘
```

### 5. Presentation concept for stakeholders
```
┌─────────────────────────────────────────────────────────┐
│ 📊 Presentation concept — non-technical stakeholders    │
│─────────────────────────────────────────────────────────│
│ 1  Today your team spends 24 hrs/month on a process     │
│    that a Power Automate flow can handle in minutes.    │
│                                                         │
│ 2  The automation connects your existing tools —        │
│    Outlook, SAP, SharePoint — no new systems needed.    │
│                                                         │
│ 3  AI Builder reads invoices automatically, reducing    │
│    manual entry errors by an estimated 90%.             │
│                                                         │
│ 4  Implementation takes ~2 weeks with no IT budget:     │
│    Power Automate is already in your M365 licence.      │
└─────────────────────────────────────────────────────────┘
```

---

## 🚀 How to run

### Option A — GitHub Pages (no setup needed)
Open the live demo: **`https://YOUR_USERNAME.github.io/mb-ai-process-analyzer`**

1. Enter your Anthropic API key (free at [console.anthropic.com](https://console.anthropic.com))
2. Paste or choose a business process example
3. Click **Analyze process with AI**

### Option B — Run locally
```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/mb-ai-process-analyzer.git
cd mb-ai-process-analyzer

# Open in browser — no server needed, it's pure HTML
open mercedes_process_analyzer.html    # macOS
start mercedes_process_analyzer.html   # Windows
```

---

## 🔑 API Key setup

This tool calls the [Anthropic Claude API](https://docs.anthropic.com) directly from your browser.

1. Create a free account at [console.anthropic.com](https://console.anthropic.com)
2. Go to **API Keys** → **Create Key**
3. Paste the key (`sk-ant-...`) into the tool's key field
4. Your key is never stored or sent anywhere — it lives only in your browser session

> **Cost:** A typical analysis uses ~800 tokens ≈ €0.002. A full demo session costs less than €0.05.

---

## 🛠️ Tech stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML, CSS, JavaScript — zero dependencies |
| AI engine | Claude Sonnet (Anthropic API) |
| Deployment | GitHub Pages — static, no backend needed |
| Automation concepts | Microsoft Power Automate, Copilot, AI Builder |

---

## 💼 Business use cases included

Click any chip in the tool to load a pre-filled example:

- **Invoice approval workflow** — Procurement, SAP, email-based approvals
- **Supplier onboarding** — Document collection, ERP entry, welcome process
- **Quality report generation** — Shift data, KPI calculation, manager distribution
- **Meeting notes & follow-ups** — Minutes, action tracker, calendar invites

---

## 🔗 Related projects

| Project | Description | Tech |
|---------|-------------|------|
| [Vita Twin AI](#) | Digital health twin — AI agent with personalized recommendations | Python, LLM, RAG |
| [Med Q&A Assistant](#) | Medical chatbot for non-technical users (doctors) | LangChain, Vector DB, NLP |
| **This tool** | Business process automation analyzer | Claude API, Power Automate |

---

## 👤 Author

Built by [Your Name] · Masters in Informatics & ML  
[LinkedIn](#) · [GitHub](#)

*Created as a Proof-of-Concept for the Mercedes-Benz KI & Automatisierung Praktikum application.*
