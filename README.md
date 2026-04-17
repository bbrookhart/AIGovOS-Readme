# AIGovOS

AIGovOS is an AI governance operating system for registering AI systems, assessing use cases, assigning risk tiers, mapping required controls, routing approvals, attaching evidence, and generating audit-ready governance summaries. It is designed to demonstrate how AI governance can be operationalized as a repeatable system of record rather than treated as a policy-only exercise.

## Why this project exists

Most organizations do not fail AI governance because they lack principles. They fail because they lack structure, ownership, evidence, and enforceable workflow.

AIGovOS is a portfolio-grade implementation of governance engineering. It is built to show how an organization can:

- maintain an inventory of AI systems
- document intended use and operating context
- assign accountable owners
- assess risk in a structured way
- map systems to required internal controls
- route approvals and exceptions
- preserve evidence for audit and review
- maintain an immutable audit trail of governance decisions

## v1 Scope

AIGovOS v1 includes:

- AI system registry
- use-case intake
- risk tiering
- control mapping
- owner assignment
- approval workflow
- evidence attachment metadata
- audit log
- exportable governance summary

## Non-goals for v1

AIGovOS v1 does **not** include:

- live model scanning
- automated vendor due diligence
- incident management workflows
- procurement approvals
- board reporting and analytics
- real-time policy enforcement inside production inference pipelines
- red-team orchestration or model evaluation harnesses

## Core Actors

- **System Owner** — accountable for the AI system and its intended use
- **Reviewer** — evaluates submissions, risks, controls, and evidence
- **Approver** — issues final decisions or conditional approvals
- **Auditor** — reviews history, rationale, and evidence
- **Admin** — manages control library, roles, and reference data

## Primary Objects

- **AI Asset** — the governed AI system or capability
- **Use Case** — a specific proposed or active use of an AI asset
- **Risk Assessment** — the structured evaluation of risk and residual risk
- **Control** — a defined governance, legal, security, privacy, or assurance requirement
- **Control Mapping** — the relationship between a use case and required controls
- **Approval Decision** — the final governance disposition
- **Evidence Artifact** — supporting documentation or proof
- **Audit Event** — a material event recorded in the governance trail

## Example Workflow

1. Register an AI asset
2. Submit a use case
3. Assign owners
4. Run risk tiering
5. Select required controls
6. Upload evidence
7. Review and approve, approve with conditions, reject, or archive
8. Export a governance summary for audit or leadership review

## System Design

### Frontend
- Next.js
- TypeScript
- Tailwind CSS

### Backend
- FastAPI
- Python
- SQLAlchemy
- Alembic

### Data
- PostgreSQL

### App Characteristics
- role-aware workflows
- auditable state changes
- evidence-first design
- explainable decisions
- narrow v1 scope

## Local Development

Setup instructions will be added as implementation begins.

Planned local workflow:

1. copy `.env.example` to `.env`
2. start Postgres with Docker Compose
3. install web and API dependencies
4. run migrations
5. start API and web apps

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
