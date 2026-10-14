<div align="center">

<img src="assets/avatar-sketch.jpg" width="140" alt="Pencil sketch of Han Dao" />

# Dao Thuy Bao Han

**Business Analyst · ERP, Fintech & EdTech**

*I go backstage to see how a business really runs, then write the setlist a dev team can play from:*
*As-Is / To-Be, BRD, UI, UAT and go-live.*

[![Portfolio](https://img.shields.io/badge/Backstage%20Pass-portfolio-C1CFA1?style=for-the-badge&labelColor=23281F)](https://dao-thuy-bao-han.kamila-comme.workers.dev)
[![Email](https://img.shields.io/badge/Email-baohandao2303%40gmail.com-E7CCCC?style=for-the-badge&logo=gmail&logoColor=23281F&labelColor=23281F)](mailto:baohandao2303@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Han%20Dao-A5B68D?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=23281F)](https://www.linkedin.com/in/h%C3%A2n-%C4%91%C3%A0o-0b12b72a3/)
[![Location](https://img.shields.io/badge/Base-Ho%20Chi%20Minh%20City-D9B1AB?style=for-the-badge&labelColor=23281F)](#)

</div>

---

## 🎟️ Backstage pass

| | |
|---|---|
| **Full BA lifecycle** | discovery → BRD → UI → UAT → go-live, since 2023 |
| **4 industries** | ERP · Fintech · EdTech · Data |
| **Now** | Business Analyst at Geta Technology — Geta Finance (ERP) and Geta Media (sales & content portal) |
| **Education** | B.Sc. Computer Science, Ton Duc Thang University (2022 – 2026) |

**How I work** — every project starts from the problem, not the feature list:

```mermaid
flowchart LR
    A[Discovery<br/>stakeholders] --> B[As-Is<br/>how it really runs]
    B --> C{Gap<br/>root cause}
    C --> D[To-Be<br/>process + rules]
    D --> E[BRD / SRS<br/>use cases · RTM]
    E --> F[UI in Figma<br/>validated flows]
    F --> G[UAT<br/>Gherkin criteria]
    G --> H((Go-live))
```

---

## 🎤 The tour — experience

### Geta Technology · Business Analyst · *May 2026 → now*
A multi-industry group selling across **8 business lines** through **83 Facebook fanpages** and Zalo. I own requirements and quality for its two internal products.

- **The problem:** 83 inboxes with no single view, one customer scattered across pages, the same price questions typed by hand, orders written up twice, and finance built from separate spreadsheets.
- **Geta Media** — one portal, one sign-in, 9 tools: a shared inbox for every fanpage and Zalo, one profile per customer (merged by phone number), a bot with 3 modes that **never invents a price**, and chat → appointment → quote → invoice in a few clicks. Content (AI rewrite → human approval → Fanpage, YouTube, TikTok) and WordPress SEO fixes all pass the same approval gate.
- **Geta Finance (ERP)** — 7 role-based workspaces behind one login: Admin, Accounting, Warehouse, Employee, Field sales, Tasks and Orders (7 stages from site measurement to handover). Orders confirmed in Geta Media flow straight into it as signed events.
- Designed the workflow for an AI multi-agent system (1 orchestrator + 3 sub-agents) with guardrails: drafts queued for approval, unusual amounts blocked in code, no tools to delete or move money.

```mermaid
flowchart LR
    subgraph Channels
      FB[83 fanpages]
      ZL[Zalo]
      WP[WordPress sites]
      TT[TikTok · YouTube]
    end
    Channels --> P[Geta Media portal<br/>one sign-in · role-based tabs]
    P --> S[Sales & care<br/>inbox · CRM · bot]
    P --> C[Content<br/>AI draft · schedule]
    P --> W[Web & SEO<br/>audit · fixes]
    S & C & W --> G{{Human approval gate}}
    G --> O[Appointment → quote → invoice]
    O -- signed order --> ERP[(Geta Finance ERP<br/>7 workspaces)]
```

### International Link Corporation (Saigon Language School) · BA & Tester · *May 2025 → May 2026*
Replaced file-based operations — spreadsheets and shared OneDrive folders for **60+ instructors, ~4,000 learners and 30 corporate classes** — with one platform.
- Traced two business risks to their root cause: **instructor double-booking** and **file access never revoked** for leavers.
- Authored the BRD end to end: **40 functional requirements, 9 business rules, 8 NFRs across 7 modules, 9 actor roles**, MoSCoW-ranked and traced in an RTM — including rules that block double-booking at scheduling time and tie data access to roles.

### PiStudy Education and Solution JSC · BA & UI/UX Designer (freelance) · *Aug 2025 → Jan 2026*
Turned **6 K-12 programs into one product** with two very different ways in — student self-signup and provisioned teacher / institution accounts — on one user model. Designed the sign-up and login UI with its validation rules in Figma. **Live at Huỳnh Khương Ninh Secondary School, ~1,000 students across 4 grades.**

### MindX Technology School · Coding & Robotics Instructor · *Mar 2024 → now*
~30 classes, ~210–240 students aged 4–18, **100% course completion**. Sole point of contact for parents: flag students early, agree a support plan, check it worked — the same loop a BA runs with stakeholders.

### Pulse Active · Data Analyst Intern · *2023 → 2024*
Cleaned and cross-checked registration data for marathons of **10,000+ and 9,000+ runners**, catching duplicates and payment mismatches before race day; built the dashboards leadership used for go / no-go decisions.

---

## 🎬 The B-sides — projects

<div align="center">

<a href="https://github.com/handao2303/tech-store-cross-platform"><img src="assets/techstore-demo.gif" width="600" alt="Tech Store Android app walkthrough: product list, best sellers and product cards" /></a>

<sub>▶ <b>Now screening</b> · Tech Store — the Android app, live on one Firestore source of truth</sub>

</div>

| Project | Problem → outcome | |
|---|---|---|
| **Banking Automation** · Lead BA | Manual KYC, Excel reconciliation and card limits with no concurrency control → a BRD that automates all three: **30 requirements, 18 use cases, 26 business rules, 18 Gherkin stories**. AML/PEP rule independent and non-overridable; the race-condition risk turned into a measurable **< 2 s SLA**. Circular 17/2024/TT-NHNN, ISO 20022 / 8583, PCI DSS. | eKYC demo on the [portfolio](https://dao-thuy-bao-han.kamila-comme.workers.dev) |
| **[Library Management](https://github.com/handao2303/library-management-system)** | Business rules (borrow quotas, FIFO approval, penalties) turned into a layered test strategy: **42 unit, 17 integration / E2E, 14 exploratory** cases in CI. Found and fixed a privilege escalation, a broken-access-control gap and an integer overflow in a DB trigger. | NestJS · React · GitHub Actions |
| **[Tech Store](https://github.com/handao2303/tech-store-cross-platform)** | Web admin + native Android app on one Firestore source of truth: 4 services, Stripe checkout, real-time stock, chat and campaigns — documented as an architecture dossier. | React · Express · Android · Firebase |
| **[TaskFlow](https://github.com/handao2303/taskflow-saas-metrics)** | A raw Stripe-style ledger → 8 SaaS metrics reconciled to **$0 variance**. Finding: MRR **~70x** but NRR only **98.7%**; Referral LTV:CAC **28.7 : 1** vs Paid Ads 2.0 : 1. Written as Finding → So what → Recommendation. | Python · pandas · Streamlit |

---

## 🧰 Toolkit

**Analysis** &nbsp;
![Elicitation](https://img.shields.io/badge/Requirements%20Elicitation-C1CFA1?style=flat-square)
![As-Is/To-Be](https://img.shields.io/badge/As--Is%20%2F%20To--Be-C1CFA1?style=flat-square)
![BRD/SRS](https://img.shields.io/badge/BRD%20%2F%20SRS-C1CFA1?style=flat-square)
![Use cases](https://img.shields.io/badge/Use%20Cases%20%26%20User%20Stories-C1CFA1?style=flat-square)
![Business rules](https://img.shields.io/badge/Business%20Rules%20%26%20Decision%20Tables-C1CFA1?style=flat-square)
![MoSCoW](https://img.shields.io/badge/MoSCoW-A5B68D?style=flat-square)
![RTM](https://img.shields.io/badge/RTM-A5B68D?style=flat-square)
![Gherkin](https://img.shields.io/badge/Gherkin%20Acceptance%20Criteria-A5B68D?style=flat-square)
![UAT](https://img.shields.io/badge/UAT-A5B68D?style=flat-square)
![Agile](https://img.shields.io/badge/Agile%20%2F%20Scrum-A5B68D?style=flat-square)

**Tools** &nbsp;
![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white)
![Confluence](https://img.shields.io/badge/Confluence-172B4D?style=flat-square&logo=confluence&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![draw.io](https://img.shields.io/badge/draw.io-F08705?style=flat-square&logo=diagramsdotnet&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![React](https://img.shields.io/badge/React-087EA4?style=flat-square&logo=react&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

**Certifications** — Google Data Analytics: Foundations · Agile Scrum Master (Techbase Vietnam)

---

<div align="center">

*Got a product that needs a BA who goes backstage?*
**[Send me the brief →](mailto:baohandao2303@gmail.com)** &nbsp;·&nbsp; **[See the full show →](https://dao-thuy-bao-han.kamila-comme.workers.dev)**

</div>
