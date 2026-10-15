<div align="center">

<a href="https://dao-thuy-bao-han.kamila-comme.workers.dev"><img src="assets/profile-card.gif" width="300" alt="About me card: Han Dao, Business Analyst — user stories, workflow optimization" /></a>

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

## 🎟️ At a glance

| | |
|---|---|
| **Role** | Business Analyst — discovery → BRD → UI → UAT → go-live |
| **Industries** | ERP · Fintech · EdTech · Data |
| **Now** | Business Analyst at **Geta Technology** — Geta Finance (ERP) and Geta Media (sales & content portal) |
| **Proof in numbers** | 3 BRDs · 40 + 30 requirements · 35 business rules · 18 use cases · 18 Gherkin stories · a platform live for ~1,000 students |
| **Education** | B.Sc. Computer Science, Ton Duc Thang University (2022 – 2026) |

### How I work
Every engagement starts from the problem, not the feature list — and every requirement stays traceable to the test that proves it.

```mermaid
flowchart LR
    subgraph U["1 · Understand"]
      direction TB
      A["Discovery<br/>stakeholder interviews"]:::in --> B["As-Is<br/>how it really runs"]:::in --> C{"Gap<br/>root cause"}:::hub
    end
    subgraph SP["2 · Specify"]
      direction TB
      D["To-Be<br/>process + business rules"]:::step --> E["BRD / SRS<br/>use cases · MoSCoW · RTM"]:::step --> F["UI in Figma<br/>validated flows"]:::step
    end
    subgraph V["3 · Validate & ship"]
      direction TB
      G["UAT<br/>Gherkin acceptance criteria"]:::step --> H(["Go-live"]):::out
    end
    U --> SP --> V
    V -. "defect → fix → retest" .-> SP
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
    style U fill:#FAFAF7,stroke:#D6DCD5
    style SP fill:#FAFAF7,stroke:#D6DCD5
    style V fill:#FAFAF7,stroke:#D6DCD5
```

---

## 🎤 Experience

### Geta Technology — Business Analyst · *May 2026 → now*
A multi-industry group (F&B, advertising, interior) selling across **8 business lines** through **83 Facebook fanpages** and Zalo. I own requirements and quality for its two internal products.

**Problem** — 83 inboxes with no single view; one customer scattered across pages; the same price questions typed by hand; every confirmed order re-entered 2–3 times; stock, sales, cash, timekeeping and payroll in separate spreadsheets.

- **Geta Media** — one portal, one sign-in, 9 tools: a shared inbox for every fanpage and Zalo, one profile per customer (merged by phone number), a bot with 3 modes that **never quotes a price on its own**, and chat → appointment → quote → invoice in a few clicks. AI-written content and website fixes pass the same human approval gate.
- **Geta Finance (ERP)** — mapped the operating flow *Inventory → Sales & Revenue → Income & Expense → Timekeeping → Payroll* and split it into **7 role-based workspaces**; each order moves through **7 stages** from site measurement to handover.
- **Media → ERP contract** — confirmed orders reach the ERP as signed events (4 event types, HMAC signature, idempotency key, retries 1 → 180 min), so nothing is entered twice.
- **Quality** — functional testing and UAT before every release; fixes verified with developers to protect live finance, stock and payroll data.

```mermaid
flowchart TB
    CH["Where customers are<br/>83 fanpages · Zalo · WordPress sites · TikTok / YouTube"]:::in
    CH --> S["Sales & care<br/>inbox · CRM · bot"]:::hub
    CH --> C["Content<br/>AI draft · schedule"]:::hub
    CH --> W["Web & SEO<br/>audit · fixes"]:::hub
    S & C & W --> G{{"Geta Media · human approval gate"}}:::gate
    G --> O["Appointment → quote → invoice"]:::step
    O -- "signed order event · HMAC · retries" --> ERP
    subgraph ERP["Geta Finance — ERP, 7 role-based workspaces"]
      direction LR
      WH["Warehouse · Orders<br/>Field sales · Tasks"]:::step
      HR["Employee<br/>timekeeping · advances"]:::step
      AC["Accounting<br/>cash book · payroll"]:::hub
      AD["Admin<br/>finance overview · permissions"]:::out
      WH --> AC
      HR --> AC
      AC --> AD
    end
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
    classDef gate fill:#FFFFFF,stroke:#D9B1AB,stroke-width:2px,stroke-dasharray:5 4,color:#23281F
    style ERP fill:#FAFAF7,stroke:#D6DCD5
```

**Outcome** — one portal for all 8 business lines; a confirmed chat becomes an appointment, an invoice and an ERP order in a few clicks; finance reports come from one flow instead of spreadsheets.

### International Link Corporation (Saigon Language School) — BA & Tester · *May 2025 → May 2026*
**Problem** — scheduling, enrollment and file access for **60+ instructors, ~4,000 learners and 30 corporate classes** ran on spreadsheets and shared OneDrive folders, with no single source of truth.

- Interviewed stakeholders across **9 roles**, mapped the As-Is and traced it to two business risks: **instructor double-booking** and **file access never revoked** for leavers.
- Authored the BRD end to end — **40 functional requirements, 9 business rules, 8 NFRs, 7 modules** — prioritized with MoSCoW and traced in an RTM; designed the To-Be and full UI, validated with stakeholders before build.

```mermaid
flowchart LR
    A["As-Is<br/>spreadsheets per desk<br/>shared OneDrive"]:::in --> R1["Risk: double-booking"]:::hub
    A --> R2["Risk: access never revoked"]:::hub
    R1 --> B1["Rule: block at scheduling time"]:::step
    R2 --> B2["Rule: access tied to role"]:::step
    B1 & B2 --> BRD["BRD · 40 FR · 9 BR · 8 NFR<br/>MoSCoW · RTM"]:::step
    BRD --> T(["To-Be: one platform, 7 modules"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

### PiStudy Education and Solution JSC — BA & UI/UX Designer (freelance) · *Aug 2025 → Jan 2026*
**Problem** — six K-12 programs with no shared structure, and two very different ways in.
Consolidated **6 programs into one information architecture** and designed **2 onboarding paths** on a single user model; wireframed the sign-up / login UI with validation rules in Figma and ran functional and usability testing. **Live at Huỳnh Khương Ninh Secondary School — ~1,000 students across 4 grades.**

```mermaid
flowchart LR
    S["Students"]:::in --> P1["Self sign-up<br/>validation rules"]:::step
    T["Teachers · schools"]:::in --> P2["Provisioned accounts"]:::step
    P1 & P2 --> U["One user model<br/>one IA for 6 programs"]:::hub
    U --> L(["Live: ~1,000 students"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

### Pulse Active — Data Analyst Intern · *2023 → 2024*
Cleaned and reconciled registration data for marathons of **10,000+ and 9,000+ runners** — catching duplicates and payment mismatches **before race day** — and built the dashboards leadership used for go / no-go decisions.

<details>
<summary><b>Diagram</b></summary>

```mermaid
flowchart LR
    R["Registrations<br/>payments · 50+ group sign-ups"]:::in --> Q["Clean & cross-check<br/>duplicates · mismatches"]:::hub
    Q --> D["Dashboards<br/>trends · revenue"]:::step
    D --> G(["Go / no-go decision"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

</details>

### MindX Technology School — Coding & Robotics Instructor (part-time) · *Mar 2024 → now*
~30 classes, ~210–240 students aged 4–18, **100% course completion**. Sole point of contact for parents — the same loop a BA runs with stakeholders.

<details>
<summary><b>Diagram</b></summary>

```mermaid
flowchart LR
    O["Observe in class"]:::in --> F["Flag early<br/>students falling behind"]:::hub
    F --> P["Agree a plan<br/>with parents"]:::step
    P --> C["Check it worked"]:::step
    C --> O
    C --> R(["100% completion"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

</details>

---

## 🎬 Projects

### Banking Automation System — Lead BA
**Problem** — account opening checked by hand against disconnected CIC/AML portals; reconciliation in Excel; card limits updated in an end-of-day batch with no concurrency control.
A BRD that automates all three: **30 requirements, 18 use cases, 26 business rules, 18 Gherkin user stories**. The AML/PEP rule is independent and non-overridable; the race-condition risk became a measurable **< 2 s response SLA**. Scope: Circular 17/2024/TT-NHNN, ISO 20022 / 8583, PCI DSS. eKYC demo on the [portfolio](https://dao-thuy-bao-han.kamila-comme.workers.dev).

```mermaid
flowchart LR
    subgraph IN["Inputs"]
      I1["ID card · NFC chip · face"]:::in
      I2["Core · Napas · card schemes"]:::in
      I3["Concurrent card transactions"]:::in
    end
    subgraph EN["Automated engine"]
      E1["eKYC + CIC/AML check"]:::hub
      E2["Auto-reconciliation incl. N:1"]:::hub
      E3["Real-time limit<br/>concurrency control"]:::hub
    end
    I1 --> E1
    I2 --> E2
    I3 --> E3
    EN --- GR{{"Guardrails: AML/PEP non-overridable · < 2 s SLA"}}:::gate
    E1 --> O1(["Account opened"]):::out
    E2 --> O2(["Ledger matched"]):::out
    E3 --> O3(["Limit updated safely"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
    classDef gate fill:#FFFFFF,stroke:#D9B1AB,stroke-width:2px,stroke-dasharray:5 4,color:#23281F
    style IN fill:#FAFAF7,stroke:#D6DCD5
    style EN fill:#FAFAF7,stroke:#D6DCD5
```

### [Checkpoint](https://github.com/handao2303/checkpoint-app) — travel social app for Vietnam · [live ↗](https://checkpoint-app.space)

<div align="center">
<a href="https://checkpoint-app.space"><img src="https://raw.githubusercontent.com/handao2303/checkpoint-app/main/docs/demo/checkpoint-demo.gif" width="560" alt="Checkpoint demo: check-in map, check-in detail, trending nearby, place detail, travel profile and moments" /></a>
</div>

**Problem** — trip memories with no map, discovery not tied to location, and no reason to go again.
Check in on a map, follow journeys, earn XP and badges, and collect a stamp for every province on a digital travel passport. Product documentation in the [hub repo](https://github.com/handao2303/checkpoint-app): problem framing, a **7-phase, 16-feature roadmap** with an explicit “won’t do” list, a plan per feature and a status log kept current. Go API · React PWA · PostGIS · Cloud Run — about **$0 a month** to run.

**Source:** [docs & design](https://github.com/handao2303/checkpoint-app) · [Go backend](https://github.com/handao2303/checkpoint-app-go) · [React web](https://github.com/handao2303/checkpoint-app-reactjs) · [React Native](https://github.com/handao2303/checkpoint-app-rn) · [Flutter](https://github.com/handao2303/checkpoint-app-flutter)

```mermaid
flowchart LR
    U1["Check in<br/>GPS + photo / video"]:::in --> API
    U2["Explore<br/>hot nearby · by distance"]:::in --> API
    API["One source of truth<br/>PostGIS · XP rules engine · media pipeline"]:::hub
    API --> V1(["Personal map"]):::out
    API --> V2(["Journeys: route & distance"]):::out
    API --> V3(["Passport: a stamp per province"]):::out
    API --> V4(["Leaderboard"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

### [Library Management](https://github.com/handao2303/library-management-system) — business rules turned into tests
Borrow quotas, FIFO approval and penalties became a layered strategy of **42 unit, 17 integration / E2E and 14 exploratory** cases running on every commit. Found and fixed **3 critical defects**: a privilege escalation, a broken-access-control gap and an integer overflow in a SQL Server trigger. *NestJS · React · GitHub Actions*

<details>
<summary><b>Diagram</b></summary>

```mermaid
flowchart LR
    BR["Business rules<br/>quotas · FIFO · penalties"]:::in --> L1["42 unit"]:::step
    BR --> L2["17 integration / E2E"]:::step
    BR --> L3["14 exploratory"]:::step
    L1 & L2 & L3 --> CI{{"CI on every commit"}}:::hub
    CI --> D(["3 critical defects found & fixed<br/>regression-locked"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

</details>

### [Tech Store](https://github.com/handao2303/tech-store-cross-platform) — one source of truth for web and Android
Web admin and a native Android app on one Firestore: 4 services, Stripe checkout, real-time stock, chat and campaigns — documented as an architecture dossier. *React · Express · Android · Firebase*

<details>
<summary><b>Diagram</b></summary>

```mermaid
flowchart LR
    W["Admin web<br/>React"]:::in --> A1["admin-api"]:::step
    M["Android app<br/>Java"]:::in --> A2["mobile-api<br/>Stripe"]:::step
    A1 & A2 --> F["Firebase Auth + Firestore<br/>one source of truth"]:::hub
    F --> R(["Real time: stock · chat · campaigns"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

</details>

### [KKBox Subscription Analytics](https://github.com/handao2303/taskflow-saas-metrics) — 430M rows of billing logs, no metric pre-computed
**Problem** — revenue keeps growing, but where is it leaking, which users are worth keeping, and what should the business fix first?
MRR, churn, NRR, cohorts and LTV rebuilt from **23M payments and 410M listening logs** (32 GB → 8.2 GB Parquet with DuckDB), with every metric definition and analysis decision written down. Findings: MRR **104.5M → 151.1M NTD (+44.5%)** yet NRR **94.8%** — the base shrinks ~5% a month; **15% of paid churn is payment-partner outages**, not users leaving; auto-renew users are worth **3.6×** manual payers. Tracked phase by phase in Jira — churn model and dashboard in progress. *Python · DuckDB · Parquet · Streamlit*

<div align="center">
<img src="https://raw.githubusercontent.com/handao2303/taskflow-saas-metrics/master/docs/images/mrr_bridge.png" width="680" alt="KKBox monthly MRR bridge: new, reactivation, expansion, contraction, churn and billing-gap churn" />
</div>

<details>
<summary><b>Diagram</b></summary>

```mermaid
flowchart LR
    R["Raw export<br/>23M payments · 410M logs"]:::in --> P["DuckDB pipeline<br/>Parquet · data-quality log"]:::hub
    P --> S["User × month snapshot<br/>24.9M rows"]:::step
    S --> M["MRR bridge · churn split<br/>cohorts · LTV"]:::step
    M --> F(["Finding → So what<br/>auto-renew = largest LTV lever"]):::out
    classDef in fill:#F4F5F2,stroke:#5A6A63,color:#23281F
    classDef step fill:#EDE8DC,stroke:#A5B68D,color:#23281F
    classDef hub fill:#E7CCCC,stroke:#23281F,color:#23281F
    classDef out fill:#C1CFA1,stroke:#23281F,color:#23281F
```

</details>

---

## 🧰 Toolkit

**Analysis** &nbsp;
![Elicitation](https://img.shields.io/badge/Requirements%20Elicitation-C1CFA1?style=flat-square)
![As-Is/To-Be](https://img.shields.io/badge/As--Is%20%2F%20To--Be-C1CFA1?style=flat-square)
![BRD/SRS](https://img.shields.io/badge/BRD%20%2F%20SRS-C1CFA1?style=flat-square)
![Use cases](https://img.shields.io/badge/Use%20Cases%20%26%20User%20Stories-C1CFA1?style=flat-square)
![Business rules](https://img.shields.io/badge/Business%20Rules%20%26%20Decision%20Tables-C1CFA1?style=flat-square)
![Data flow](https://img.shields.io/badge/Data%20Flow%20Modeling-C1CFA1?style=flat-square)
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

**Certifications** — Google Data Analytics: Foundations (Google) · Agile Scrum Master (Techbase Vietnam)

---

<div align="center">

*Got a product that needs a BA who goes backstage?*
**[Send me the brief →](mailto:baohandao2303@gmail.com)** &nbsp;·&nbsp; **[See the full show →](https://dao-thuy-bao-han.kamila-comme.workers.dev)**

</div>
