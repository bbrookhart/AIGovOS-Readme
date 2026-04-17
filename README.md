<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,45:1E293B,75:2563EB,100:38BDF8&height=240&section=header&text=AIGovOS&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI%20Governance%20Operating%20System&descAlignY=58&descAlign=50" alt="AIGovOS banner" />
</p>

<p align="center">
  <strong>Operational AI governance for inventory, intake, risk tiering, control mapping, approvals, evidence, and audit-ready decision records.</strong>
</p>

<p align="center">
  A portfolio-grade governance engineering platform that demonstrates how AI oversight can be implemented as a real workflow system — not policy text, slideware, or disconnected review checklists.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-in%20development-2563EB?style=for-the-badge" alt="Status" />
  <img src="https://img.shields.io/badge/focus-AI%20Governance-111827?style=for-the-badge" alt="Focus" />
  <img src="https://img.shields.io/badge/design-Audit--First-1F2937?style=for-the-badge" alt="Audit First" />
  <img src="https://img.shields.io/badge/approach-Governance%20Engineering-0F172A?style=for-the-badge" alt="Governance Engineering" />
</p>

---

## Table of Contents

- [Overview](#overview)
- [Why This Project Exists](#why-this-project-exists)
- [Core Value Proposition](#core-value-proposition)
- [Technology Stack](#technology-stack)
- [What AIGovOS Does](#what-aigovos-does)
- [Design Principles](#design-principles)
- [v1 Scope](#v1-scope)
- [Governance Workflow](#governance-workflow)
- [Core Actors](#core-actors)
- [Core Objects](#core-objects)
- [Architecture](#architecture)
- [Demo Scenarios](#demo-scenarios)
- [Key Features](#key-features)
- [Repository Structure](#repository-structure)
- [Local Development](#local-development)
- [Roadmap](#roadmap)
- [Definition of Done for v1](#definition-of-done-for-v1)
- [Portfolio Positioning](#portfolio-positioning)
- [License](#license)

---

## Overview

AIGovOS is an **AI governance operating system** built to show how organizations can move from abstract principles to concrete governance workflows.

Instead of treating AI governance as a static policy artifact, AIGovOS treats it as an operational discipline covering:

- System inventory
- Structured use-case intake
- Risk classification
- Control assignment
- Accountable ownership
- Evidence attachment
- Approval decisions
- Auditability
- Exportable governance summaries

This project is designed to signal capability across AI governance, ethical GRC, AI risk management, governance workflow design, control engineering, evidence management, approval systems, auditable oversight, and operational responsible AI.

---

## Why This Project Exists

Most organizations do not fail AI governance because they lack principles. They fail because they lack:

- An accurate inventory of AI systems
- A repeatable intake process for new AI use cases
- Clear owners and reviewers
- Consistent risk tiering
- Mapped control requirements
- Structured evidence collection
- Formal approval records
- Audit-ready decision history

AIGovOS exists to close that gap. It demonstrates that modern AI governance is not just policy writing — it is the design of systems that can classify AI use, assign responsibility, require controls, preserve rationale, record decisions, and prove governance happened.

---

## Core Value Proposition

AIGovOS operationalizes governance as a workflow system of record. It allows a team to:

1. Register an AI system
2. Define how that system will be used
3. Assess the governance risk of that use
4. Determine what controls are required
5. Attach evidence supporting approval
6. Approve, conditionally approve, reject, or archive
7. Preserve an audit trail of who did what and why
8. Export a governance summary for review or audit

This makes AIGovOS directly relevant to Responsible AI, AI governance, AI assurance, technology risk, ethical GRC, AI policy operationalization, digital trust, compliance engineering, and regulated AI oversight.

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

### Data & Infrastructure

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white" alt="pnpm" />
  <img src="https://img.shields.io/badge/Makefile-1D3557?style=for-the-badge&logo=gnu&logoColor=white" alt="Makefile" />
</p>

### API & Engineering

<p>
  <img src="https://img.shields.io/badge/OpenAPI-6BA539?style=for-the-badge&logo=openapiinitiative&logoColor=white" alt="OpenAPI" />
  <img src="https://img.shields.io/badge/Monorepo-111827?style=for-the-badge" alt="Monorepo" />
  <img src="https://img.shields.io/badge/Auditability-First-1F2937?style=for-the-badge" alt="Auditability First" />
  <img src="https://img.shields.io/badge/Workflow-Driven-374151?style=for-the-badge" alt="Workflow Driven" />
  <img src="https://img.shields.io/badge/Evidence-Centric-2563EB?style=for-the-badge" alt="Evidence Centric" />
</p>

---

## What AIGovOS Does

| Capability | Description |
| --- | --- |
| **AI Asset Registry** | Tracks governed AI systems, models, assistants, tools, and automations |
| **Use-Case Intake** | Captures intended purpose, operating context, exposure type, data sensitivity, and oversight |
| **Risk Tiering** | Applies deterministic governance rules to classify use-case scrutiny |
| **Control Mapping** | Assigns required governance controls based on risk and context |
| **Evidence Tracking** | Links supporting artifacts, notes, and review materials to decisions |
| **Approval Workflow** | Supports approval, conditional approval, rejection, and archival |
| **Audit Trail** | Records material workflow actions and rationale |
| **Governance Export** | Produces structured governance summaries for audit or stakeholder review |

---

## Design Principles

AIGovOS is built around a small set of strong design principles:

- **Governance before analytics**
- **Workflow before dashboard**
- **Evidence before claims**
- **Deterministic logic before opaque scoring**
- **Auditability as a core feature**
- **Clear ownership before automation**
- **Narrow scope before expansion**

---

## v1 Scope

### In Scope

- AI asset registry
- Use-case intake
- Owner assignment
- Deterministic risk tiering
- Control mapping
- Approval workflow
- Evidence artifact tracking
- Audit event logging
- Exportable governance summary

### Out of Scope for v1

To keep the first release tight, credible, and portfolio-ready, v1 does **not** include:

- Vendor due diligence workflows
- Automated model benchmarking
- Prompt injection testing
- Incident and harm management
- Procurement approvals
- Executive dashboards
- Real-time production enforcement
- Multi-tenant SaaS isolation
- Advanced notification or escalation systems

---

## Governance Workflow

AIGovOS follows a clean governance lifecycle:

```text
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

### Supported Workflow States

- `Draft`
- `Submitted`
- `Under Review`
- `Approved`
- `Approved with Conditions`
- `Rejected`
- `Archived`

This keeps governance state explicit, reviewable, and easy to explain.

---

## Core Actors

| Actor | Responsibility |
| --- | --- |
| **System Owner** | Accountable for the AI asset and its intended use |
| **Reviewer** | Validates use-case information, assesses risk, reviews controls, and checks evidence |
| **Approver** | Issues the final governance disposition |
| **Auditor** | Reviews records, rationale, and traceability without changing workflow state |
| **Admin** | Maintains controls, platform configuration, and governance reference data |

---

## Core Objects

AIGovOS centers on a small set of governance objects:

| Object | Purpose |
| --- | --- |
| **AI Asset** | A governed system, model, assistant, or automation |
| **Use Case** | A specific proposed or active use of an AI asset |
| **Owner** | The accountable actor in the workflow |
| **Risk Assessment** | Structured governance risk record with rationale |
| **Control** | A governance requirement that applies based on context |
| **Control Mapping** | The relationship between a use case and required controls |
| **Approval Decision** | Formal governance disposition and rationale |
| **Evidence Artifact** | Supporting documentation or linked proof |
| **Audit Event** | Append-only record of material workflow activity |

---

## Architecture

### High-Level System View

```text
┌──────────────────────────────────────────────────────────────┐
│                           AIGovOS                            │
├──────────────────────────────────────────────────────────────┤
│ Web App                                                      │
│ Next.js • React • TypeScript • Tailwind CSS                  │
│                                                              │
│ - AI asset registry                                          │
│ - Use-case intake                                            │
│ - Reviewer workflow                                          │
│ - Approval panel                                             │
│ - Evidence views                                             │
│ - Audit history                                              │
├──────────────────────────────────────────────────────────────┤
│ API Service                                                  │
│ FastAPI • Python • Pydantic • SQLAlchemy • Alembic           │
│                                                              │
│ - Request validation                                         │
│ - Persistence                                                │
│ - Risk tiering                                               │
│ - Control selection                                          │
│ - Approval validation                                        │
│ - Audit event creation                                       │
│ - Governance summary export                                  │
├──────────────────────────────────────────────────────────────┤
│ Database                                                     │
│ PostgreSQL                                                   │
│                                                              │
│ - Workflow state                                             │
│ - Governance objects                                         │
│ - Approval history                                           │
│ - Audit records                                              │
└──────────────────────────────────────────────────────────────┘
```

### Architecture Philosophy

The frontend is responsible for **workflow presentation**. The backend is responsible for **governance truth**.

That means:

- The frontend renders forms, lists, and actions
- The backend decides risk tiering
- The backend assigns required controls
- The backend validates approval preconditions
- The backend creates authoritative audit events

This preserves integrity, testability, and a stronger governance signal.

### Why This Architecture Matters

AIGovOS is not an inference product — it is a governance system. That changes the architectural priorities. The most important integrity concerns are:

- Broken access control
- Unauthorized approval
- Workflow bypass
- Audit log integrity
- Evidence tampering
- Export overexposure
- Traceable actor identity

Because of that, the backend is designed to own workflow state transitions, approval validation, control selection, and audit creation. That is what makes the project credible from a governance and GRC perspective.

---

## Demo Scenarios

AIGovOS is designed around three demo scenarios that create a strong narrative arc.

### 1. Internal Meeting Summarizer

A low-risk internal productivity workflow.

> **Why it matters:** Shows proportional governance for ordinary internal AI use.

### 2. Creator Support Chatbot

A medium-risk external-facing assistant.

> **Why it matters:** Shows stronger review, evidence, and conditional approval for public-facing AI.

### 3. Synthetic Voice Rights Review Tool

A high-scrutiny governance scenario tied to synthetic identity, likeness, and creative rights.

> **Why it matters:** Differentiates the portfolio by showing how AIGovOS can support serious review of sensitive AI uses with legal, ethical, and reputational stakes.

---

## Key Features

| Feature | Description |
| --- | --- |
| **Inventory** | Track AI systems, capabilities, and governed assets in a central registry |
| **Intake** | Capture intended purpose, deployment context, exposure type, affected users, and oversight details |
| **Risk Tiering** | Apply explainable governance rules to classify use-case scrutiny |
| **Control Mapping** | Assign required controls based on use-case attributes and risk tier |
| **Evidence** | Attach supporting documentation, notes, disclosures, and safeguards summaries |
| **Approvals** | Issue formal decisions with rationale, including conditional approvals |
| **Auditability** | Record material workflow actions and preserve decision traceability |
| **Exports** | Generate governance summaries for internal review or audit preparation |

---

## Repository Structure

```text
aigovos/
├── README.md
├── LICENSE
├── .gitignore
├── .editorconfig
├── .env.example
├── Makefile
├── docker-compose.yml
├── pnpm-workspace.yaml
├── package.json
├── docs/
│   ├── architecture.md
│   ├── scope.md
│   ├── control-mapping.md
│   ├── approval-workflow.md
│   ├── data-model.md
│   ├── api-contract.md
│   ├── threat-model.md
│   ├── decision-log.md
│   └── demo-scenarios.md
├── apps/
│   ├── web/
│   └── api/
└── packages/
    ├── ui/
    ├── config/
    └── types/
```

### Planned API Capabilities

The API will support:

- AI asset CRUD
- Use-case creation and submission
- Risk assessment retrieval and recomputation
- Control mapping generation
- Evidence artifact management
- Approval decisions
- Audit event queries
- Exportable governance summaries

### Backend Responsibilities

The backend is the authoritative layer for:

- Workflow transitions
- Risk logic
- Control enforcement
- Approval validation
- Audit generation

This is a deliberate design choice. Governance decisions should not depend on frontend logic.

---

## Screenshots

> _Screenshots will be added here once the first end-to-end workflow is implemented._

Planned screenshot sections:

- Dashboard
- AI asset registry
- Use-case intake form
- Risk assessment panel
- Control mapping view
- Approval panel
- Audit trail
- Export summary

---

## Local Development

### Prerequisites

- Node.js
- pnpm
- Python 3.11+
- Docker
- Docker Compose

### Planned Setup

```bash
cp .env.example .env
docker compose up -d postgres
pnpm install
make dev
```

### Planned Service URLs

| Service | URL |
| --- | --- |
| Web app | `http://localhost:3000` |
| API | `http://localhost:8000` |
| OpenAPI docs | `http://localhost:8000/docs` |

---

## Roadmap

### v1

- AI asset registry
- Use-case intake
- Risk tiering
- Control mapping
- Approvals
- Evidence metadata
- Audit log
- Exports

### v1.1

- File upload support
- PDF exports
- Notification layer
- Stronger RBAC

### v2

- Vendor AI risk module
- Incident and near-miss register
- Policy exception workflows
- Executive governance reporting
- Domain-specific governance profiles

---

## Definition of Done for v1

AIGovOS v1 is complete when a user can:

- [x] Register an AI asset
- [x] Create a use case
- [x] Assign ownership
- [x] Calculate a risk tier
- [x] Generate required controls
- [x] Attach supporting evidence
- [x] Issue a decision with rationale
- [x] Inspect the audit trail
- [x] Export a governance summary

---

## Portfolio Positioning

AIGovOS is built to show that AI governance is not just documentation. It is the design of systems that can:

- Classify AI use
- Assign responsibility
- Enforce governance expectations
- Preserve evidence
- Record why something was approved
- Demonstrate what happened, when, and by whom

That is the difference between **policy awareness** and **governance engineering**.

### Future Expansion Areas

The current design intentionally leaves room for later modules such as:

- Third-party AI risk and procurement review
- Incident and harm register
- Policy exception workflows
- Executive governance reporting
- Domain-specific governance overlays
- Creative-IP and digital replica governance profiles

---

## Author

Built as a portfolio and governance-engineering project focused on:

- AI governance
- Ethical GRC
- Auditable decision systems
- Operational responsible AI
- Governance workflow design

---

## License

This project is licensed under the [MIT License](LICENSE).

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:38BDF8,25:2563EB,55:1E293B,100:0F172A&height=120&section=footer" alt="footer" />
</p>
