# AIGovOS

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,45:1E293B,75:2563EB,100:38BDF8&height=240&section=header&text=AIGovOS&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI%20Governance%20Operating%20System&descAlignY=58&descAlign=50" alt="AIGovOS banner" />
</p>

<p align="center">
  <strong>Operational AI governance — inventory, intake, risk tiering, control mapping, approvals, evidence, and audit-ready decision records.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-in%20development-2563EB?style=for-the-badge" alt="Status" />
  <img src="https://img.shields.io/badge/focus-AI%20Governance-111827?style=for-the-badge" alt="Focus" />
  <img src="https://img.shields.io/badge/design-Audit--First-1F2937?style=for-the-badge" alt="Audit First" />
  <img src="https://img.shields.io/badge/approach-Governance%20Engineering-0F172A?style=for-the-badge" alt="Governance Engineering" />
</p>

---

## What It Is

AIGovOS is a **governance workflow system** that operationalizes AI oversight as a real engineering discipline rather than policy text or disconnected review checklists.

Most organizations don't fail at AI governance because they lack principles. They fail because they lack:

- an accurate inventory of AI systems
- a repeatable intake process for new use cases
- clear owners and reviewers
- consistent risk tiering
- mapped control requirements
- structured evidence collection
- formal approval records
- audit-ready decision history

AIGovOS closes that gap — built to show that governance is the design of systems that can classify AI use, assign responsibility, preserve rationale, and prove that oversight happened.

---

## What It Does

| Capability | Description |
|---|---|
| **AI Asset Registry** | Track governed systems, models, assistants, tools, and automations |
| **Use-Case Intake** | Capture intended purpose, operating context, exposure type, data sensitivity, and oversight structure |
| **Risk Tiering** | Apply deterministic, explainable rules to classify use-case scrutiny |
| **Control Mapping** | Assign required governance controls based on risk tier and context |
| **Evidence Tracking** | Link supporting artifacts, notes, and review materials to decisions |
| **Approval Workflow** | Issue formal dispositions — approved, conditionally approved, rejected, or archived |
| **Audit Trail** | Append-only record of material workflow actions and rationale |
| **Governance Export** | Produce structured summaries for internal review or audit preparation |

---

## Governance Workflow

```
Register AI Asset
       ↓
Submit Use Case
       ↓
Assign Owner / Reviewer
       ↓
Run Risk Tiering
       ↓
Generate Required Controls
       ↓
Attach Evidence
       ↓
Review and Decide
       ↓
Record Audit Trail
       ↓
Export Governance Summary
```

**Supported Workflow States:** `Draft` → `Submitted` → `Under Review` → `Approved` / `Approved with Conditions` / `Rejected` / `Archived`

---

## Core Actors

| Role | Responsibility |
|---|---|
| **System Owner** | Accountable for the AI asset and its intended use |
| **Reviewer** | Validates intake, assesses risk, reviews controls and evidence |
| **Approver** | Issues the final governance disposition |
| **Auditor** | Inspects records and rationale without modifying workflow state |
| **Admin** | Maintains controls, reference data, and platform configuration |

---

## Core Objects

| Object | Purpose |
|---|---|
| **AI Asset** | A governed system, model, assistant, or automation |
| **Use Case** | A specific proposed or active use of an AI asset |
| **Risk Assessment** | Structured governance risk record with rationale |
| **Control** | A governance requirement that applies based on context |
| **Control Mapping** | Relationship between a use case and its required controls |
| **Approval Decision** | Formal governance disposition and rationale |
| **Evidence Artifact** | Supporting documentation or linked proof |
| **Audit Event** | Append-only record of material workflow activity |

---

## Technology Stack

### Frontend
<p>
  <img src="https://img.shields.io/badge/Next.js-15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/React-19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
</p>

### Backend
<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white" alt="Pydantic" />
  <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white" alt="SQLAlchemy" />
  <img src="https://img.shields.io/badge/Alembic-222222?style=for-the-badge&logo=python&logoColor=white" alt="Alembic" />
</p>

### Data and Infrastructure
<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white" alt="pnpm" />
</p>

---

## Architecture

```
┌──────────────────────────────────────────────────────────────┐
│ Web App  —  Next.js • React • TypeScript • Tailwind CSS      │
│                                                              │
│  AI asset registry  •  use-case intake  •  reviewer         │
│  workflow  •  approval panel  •  evidence  •  audit history  │
├──────────────────────────────────────────────────────────────┤
│ API Service  —  FastAPI • Python • Pydantic • SQLAlchemy     │
│                                                              │
│  risk tiering  •  control selection  •  approval            │
│  validation  •  audit event creation  •  export             │
├──────────────────────────────────────────────────────────────┤
│ Database  —  PostgreSQL                                      │
│                                                              │
│  workflow state  •  governance objects  •  audit records     │
└──────────────────────────────────────────────────────────────┘
```

**Architecture principle:** The frontend owns workflow presentation. The backend owns governance truth — risk tiering, control assignment, approval validation, and authoritative audit events. This preserves integrity, testability, and the correct separation of concerns for a governance system.

---

## Design Principles

- Governance before analytics
- Workflow before dashboard
- Evidence before claims
- Deterministic logic before opaque scoring
- Auditability as a core feature, not an afterthought
- Clear ownership before automation
- Narrow scope before expansion

---

## Repository Structure

```
aigovos/
├── README.md
├── LICENSE
├── .env.example
├── Makefile
├── docker-compose.yml
├── pnpm-workspace.yaml
├── docs/
│   ├── architecture.md
│   ├── scope.md
│   ├── control-mapping.md
│   ├── approval-workflow.md
│   ├── data-model.md
│   ├── api-contract.md
│   ├── threat-model.md
│   ├── decision-log.md
│   ├── demo-scenarios.md
│   ├── demo-walkthrough.md
│   └── screenshots/
├── apps/
│   ├── web/
│   └── api/
└── packages/
    ├── ui/
    ├── config/
    └── types/
```

---

## Local Development

**Prerequisites:** Node.js, pnpm, Python 3.11+, Docker, Docker Compose

```bash
cp .env.example .env
docker compose up -d postgres
pnpm install
make dev
```

| Service | URL |
|---|---|
| Web app | http://localhost:3000 |
| API | http://localhost:8000 |
| OpenAPI docs | http://localhost:8000/docs |

### Seed Data

The included demo seed script creates three end-to-end governance scenarios with owners, assets, use cases, risk assessments, control mappings, evidence artifacts, approval decisions, and audit events.

```bash
python -m app.seed.seed_demo_data
```

---

## Demo Scenarios

AIGovOS ships with three scenarios that demonstrate the full governance arc across risk tiers:

| Scenario | Risk Profile | Demonstrates |
|---|---|---|
| **Internal Meeting Summarizer** | Low | Proportional governance for ordinary internal AI use |
| **Creator Support Chatbot** | Medium | Stronger review, evidence, and conditional approval for external-facing AI |
| **Synthetic Voice Rights Review Tool** | High | Governance of sensitive AI use with legal, ethical, and reputational stakes |

See [`docs/demo-walkthrough.md`](docs/demo-walkthrough.md) for the recommended walkthrough sequence.

---

## v1 Scope

**In scope:** AI asset registry, use-case intake, owner assignment, risk tiering, control mapping, approval workflow, evidence artifact tracking, audit event logging, governance summary export.

**Out of scope for v1:** vendor due diligence, automated model benchmarking, prompt injection testing, incident and harm management, procurement approvals, executive dashboards, real-time production enforcement, multi-tenant SaaS isolation, notification and escalation systems.

### Definition of Done

v1 is complete when a user can:

1. Register an AI asset
2. Create a use case and assign ownership
3. Run risk tiering and generate required controls
4. Attach supporting evidence
5. Issue a decision with rationale
6. Inspect the full audit trail
7. Export a governance summary

---

## Roadmap

**v1.1** — File upload support, PDF exports, notification layer, stronger RBAC

**v2** — Vendor AI risk module, incident and near-miss register, policy exception workflows, executive governance reporting, domain-specific governance profiles

---

## Portfolio Positioning

AIGovOS is relevant to roles and functions involving: Responsible AI, AI governance, AI assurance, technology risk, ethical GRC, AI policy operationalization, digital trust, compliance engineering, and regulated AI oversight.

It is built as a proof-of-work signal that AI governance can be treated as an engineering discipline — not just documentation.

---

## License

MIT License
