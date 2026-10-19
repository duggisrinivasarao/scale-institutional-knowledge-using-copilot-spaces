# OctoAcme Project Management Docs

This folder contains OctoAcme’s program-level project management process documents. The files below provide a single entry point to understand how OctoAcme runs projects, who owns what, and where to find templates and checklists for initiation, planning, execution, releases, risk management, and continuous improvement.

OctoAcme follows a lightweight, iterative project management approach centered on clear outcomes and frequent, small deliveries. Projects start with a Project One-pager that captures the problem, measurable goals, stakeholders, and a rough timeline. Teams then move through planning (kickoff, prioritized backlog, estimation, and Definition of Done) into execution, release, and close/retrospective. This lifecycle helps teams validate assumptions early, deliver value in small slices, and capture learning after each milestone.

Workflows are standardized around a project board (Backlog → Ready → In Progress → In Review → QA → Done) and a disciplined pull request process: small PRs with linked issues and acceptance criteria, automated CI checks and security scans, and required approvals before merging. Key artifacts include the Project One-pager, a prioritized backlog with acceptance criteria, a Risk Register, release notes, and sprint artifacts (estimates, DoD). Release guidance prescribes pre-release checks, smoke tests in staging, rollback plans, and post-deploy verifications.

Clear roles and communication cadence ensure predictable delivery. Product Managers (PdMs) define outcomes and prioritize the backlog; Project Managers (PMs) coordinate schedules, risks, and stakeholder communication; Developers build and test features; QA validates acceptance criteria and runs integration/acceptance checks. Teams use daily standups for progress and blockers, weekly delivery syncs for updates and escalation, demo/review sessions at the end of sprints, and regular retrospectives to drive continuous improvement. Quality practices combine unit and integration tests, end-to-end smoke tests for critical flows, CI linting and security scanning, and manual QA when needed. Risks are tracked in a register with defined escalation paths and communication templates for status and incidents.

## Docs (links)
- [octoacme-project-management-overview.md](./octoacme-project-management-overview.md) — Overview and core roles
- [octoacme-project-initiation.md](./octoacme-project-initiation.md) — Project initiation guide and one-pager template
- [octoacme-project-planning.md](./octoacme-project-planning.md) — Planning activities, backlog template, risk register
- [octoacme-execution-and-tracking.md](./octoacme-execution-and-tracking.md) — Day-to-day execution, PR workflow, CI
- [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md) — Release types, deployment checklist, rollback playbook
- [octoacme-risks-and-communication.md](./octoacme-risks-and-communication.md) — Risk register and communication templates
- [octoacme-retrospective-and-continuous-improvement.md](./octoacme-retrospective-and-continuous-improvement.md) — Retrospective structure and tracking
- [octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md) — Role descriptions and responsibilities

## Maintenance notes
- Keep this README concise and update when new process docs are added or filenames change.
- Link from the project README to docs/README.md to improve discoverability.
