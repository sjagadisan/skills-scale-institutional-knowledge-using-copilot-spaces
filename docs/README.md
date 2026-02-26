# OctoAcme Project Management — Documentation Overview

Welcome to the OctoAcme project management docs. This README provides a brief orientation to how OctoAcme runs projects, so new teammates can quickly understand our approach before diving into the detailed guides.

## Project Lifecycle

OctoAcme follows a five-phase lifecycle to deliver features and services iteratively and safely.

1. **Initiation** — Validate the business need, align stakeholders, and produce a lightweight Project One-pager with problem statement, success metrics, and an initial risk list. A go/no-go decision gate determines readiness to proceed. See [Project Initiation](octoacme-project-initiation.md).
2. **Planning** — Break the approved initiative into a prioritized backlog with acceptance criteria, estimates, and a Definition of Done. Release milestones, dependencies, and an initial QA plan are agreed at this stage. See [Project Planning](octoacme-project-planning.md).
3. **Execution** — The delivery team builds, tests, and reviews work in short iterations tracked on a project board (Backlog → Ready → In Progress → In Review → QA → Done). Pull requests are kept small (≤ 400 lines), linked to issues, and must pass CI and receive at least one approval before merging. See [Execution & Tracking](octoacme-execution-and-tracking.md).
4. **Release** — Before deploying to production, all acceptance criteria must be met, CI and security scans must pass, release notes drafted, and a rollback plan documented. The deployment checklist covers staging smoke tests, production deployment, post-deploy verification, and stakeholder announcements. See [Release & Deployment](octoacme-release-and-deployment.md).
5. **Close & Retrospective** — After each sprint, release, or milestone the team reflects on what went well, what could improve, and commits to 2–3 concrete action items tracked in the backlog. See [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md).

For a high-level summary of these phases and the key artifacts produced at each stage (Project Charter, Roadmap, Sprint Backlog, Risk Register, and Retrospective notes), see the [Project Management Overview](octoacme-project-management-overview.md).

## Roles & Personas

Three core roles collaborate on every OctoAcme project. The **Project Manager (PM)** coordinates delivery activities, manages schedules, maintains the Risk Register, and facilitates ceremonies (kickoff, planning, retrospectives). The **Product Manager (PdM)** owns the product vision, prioritizes the roadmap and backlog, defines success metrics, and validates outcomes through data and user research. **Developers** implement features, write tests, participate in design and code reviews, and surface technical risks early. Additional stakeholders provide input, sign off on deliverables, and receive regular status updates. Full persona definitions, goals, and typical communication patterns are documented in [Roles & Personas](octoacme-roles-and-personas.md).

## Communication & Risk Management

OctoAcme maintains a predictable communication cadence: twice-weekly standups keep the delivery team synchronized, a weekly PM + PdM sync aligns delivery with product strategy, and monthly stakeholder updates ensure executive and cross-functional visibility. Ad-hoc escalations follow a clear path — team-level triage in standup → PM escalates to Product Lead → sponsor-level escalation for business-impacting issues. Risks are captured in a Risk Register (ID, description, impact, likelihood, owner, mitigation, status) and reviewed weekly. Incident communication follows a structured template (triage summary, actions, timeline, post-incident blameless retro). Communication templates and escalation paths are detailed in [Risk Management & Communication](octoacme-risks-and-communication.md).

## Quality Assurance

Quality is built in throughout the lifecycle rather than bolted on at the end. During execution the team writes unit tests for all new logic, integration tests where applicable, and end-to-end smoke tests for critical flows. Security scanning runs in CI on every PR. Manual QA for feature acceptance is performed when automated coverage is insufficient. Velocity, burndown, and product success metrics are tracked continuously, and dashboards monitor error rates, latency, and usage signals. Before any release, smoke tests are run in staging and a rollback/mitigation plan is documented. Detailed testing expectations and the deployment checklist can be found in [Execution & Tracking](octoacme-execution-and-tracking.md) and [Release & Deployment](octoacme-release-and-deployment.md).

---

## All Documentation

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and lifecycle summary |
| [Project Initiation](octoacme-project-initiation.md) | One-pager template, stakeholder alignment, and go/no-go gate |
| [Project Planning](octoacme-project-planning.md) | Backlog creation, estimation, DoD, and release planning |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Project board workflow, PR conventions, QA, and blocker escalation |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk Register, communication cadence, and escalation paths |
| [Release & Deployment](octoacme-release-and-deployment.md) | Release checklists, rollback playbook, and release notes template |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro structure, action item tracking, and improvement culture |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and goals for PM, PdM, and Developers |
