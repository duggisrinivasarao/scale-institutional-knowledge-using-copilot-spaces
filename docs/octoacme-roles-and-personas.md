# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (Proposed additions)

To improve clarity, accountability, and handoffs across delivery, the following personas are proposed to be added to this document. For each persona we provide a short role summary, core responsibilities, and how they interact with existing roles.

### Delivery Lead

Role summary:
- Owns day-to-day delivery execution for a project or major feature stream.

Responsibilities:
- Coordinate sprint planning and ensure backlog items are ready for delivery
- Track delivery risks, blockers, and team capacity
- Facilitate cross-functional coordination (engineering, QA, design, release)
- Drive daily standups and ensure action items are tracked

Interactions:
- Works closely with Project Manager (PM) on schedule and dependencies
- Aligns with Product Manager (PdM) on priorities and acceptance criteria
- Escalates unresolved technical blockers to Engineering Manager
- Hands off to Release Manager for deployment coordination

Expected artifacts:
- Sprint agendas, delivery risk log, status notes for weekly updates

---

### Engineering Manager

Role summary:
- Responsible for technical direction, team health, and resource allocation.

Responsibilities:
- Oversee architecture and engineering standards
- Make staffing and prioritization decisions for technical work
- Mentor engineers and manage performance and capacity
- Coordinate technical risk mitigation and technical debt management

Interactions:
- Collaborates with Delivery Lead on capacity and technical estimates
- Works with Developers on implementation details and code quality
- Provides input to PM/PdM for resource planning and feasibility

Expected artifacts:
- Capacity plans, architecture notes, technical risk register

---

### UX Researcher / Designer

Role summary:
- Owns user research, interaction design, and accessibility for features.

Responsibilities:
- Conduct user research and synthesize findings into actionable insights
- Produce design deliverables (wireframes, mockups, prototypes)
- Validate designs through usability testing and accessibility checks
- Contribute acceptance criteria around usability

Interactions:
- Works with PdM to define user goals and acceptance criteria
- Collaborates with Developers to ensure feasible implementations
- Engages QA for usability and accessibility verification

Expected artifacts:
- Research findings, design specs, accessibility checklists

---

### Release Manager

Role summary:
- Plans and coordinates releases across environments and teams.

Responsibilities:
- Define release windows, deployment runbooks, and rollback plans
- Coordinate staging verification and post-deploy checks
- Communicate release timing and impact to stakeholders and support
- Ensure release compliance (migration steps, config changes)

Interactions:
- Receives deployment readiness sign-off from Delivery Lead and QA
- Works with Observability Owner for post-release verification
- Escalates incidents to PM/On-call as needed

Expected artifacts:
- Release plan, runbooks, deployment checklist, rollback procedures

---

### Observability / Monitoring Owner

Role summary:
- Ensures the project has appropriate monitoring, SLOs, and dashboards.

Responsibilities:
- Define service-level objectives (SLOs), key metrics, and alerts
- Create dashboards for pre- and post-release verification
- Tune alerting to avoid noise and ensure actionable signals
- Support incident response and post-incident analysis

Interactions:
- Works with Developers to instrument code and validate telemetry
- Coordinates with Release Manager for verification signals after deployments
- Advises PM on measurable impact metrics where relevant

Expected artifacts:
- SLO definitions, dashboards, alert runbooks

---

### Security Representative

Role summary:
- Ensures security and compliance concerns are integrated into delivery.

Responsibilities:
- Coordinate security reviews, threat modeling, and code scans
- Ensure CI security checks and remediation are in place
- Document compliance or regulatory requirements for the project
- Advise on secure design and data handling practices

Interactions:
- Works with Developers and Engineering Manager on fixes and mitigations
- Provides acceptance criteria related to security for PdM/PM to include
- Collaborates with Release Manager for secure deployment checks

Expected artifacts:
- Threat models, security checklists, scan results and mitigation plans

---

### Business Analyst

Role summary:
- Translates stakeholder needs into clear requirements and acceptance criteria.

Responsibilities:
- Elicit and document detailed requirements and workflows
- Produce acceptance tests and examples for complex scenarios
- Help prioritize requirements and clarify scope with PdM
- Validate implemented features against business expectations

Interactions:
- Works with PdM to refine backlog items
- Collaborates with Developers and QA to ensure acceptance tests are understood and executed
- Acts as a bridge between stakeholders and the delivery team

Expected artifacts:
- Requirements docs, acceptance test cases, example data/scenarios

---

### Stakeholder Liaison / Product Sponsor Representative

role summary:
- Central point for stakeholder communications, approvals, and priority alignment.

Responsibilities:
- Maintain stakeholder expectations and communicate milestone progress
- Collect and prioritize external stakeholder feedback
- Provide timely approvals or decisions on scope changes
- Participate in key reviews and acceptance gates

Interactions:
- Works with PM and PdM for status updates and alignment
- Engages Delivery Lead for delivery implications of stakeholder requests

Expected artifacts:
- Stakeholder communications, decision logs, approval records

---

### Support / Customer Success Lead

Role summary:
- Represents operations, support, and customer-facing teams in planning and releases.

Responsibilities:
- Provide customer feedback and define support readiness criteria
- Prepare support runbooks, FAQs, and escalation guides
- Coordinate training or communications for support teams pre-release
- Track and communicate post-release customer impact

Interactions:
- Works with Release Manager on communication plans
- Collaborates with PdM/PM for priorities driven by customer needs
- Assists Observability Owner with customer-impact metrics and alerts

Expected artifacts:
- Support runbooks, customer communications, readiness checklists

---

## Integration guidance and handoffs

For each persona above, include in the project's role section:
- A short role summary and 3–5 core responsibilities
- Key interactions (who they coordinate with and handoffs)
- Common artifacts they own (e.g., runbooks, acceptance tests, dashboards)
- Suggested escalation path for blockers and incidents

Example handoff scenario:
- Delivery Lead marks a release ready and notifies Release Manager with the release checklist.
- Release Manager coordinates staging verification and tells Observability Owner which dashboards will be used for post-release verification.
- If a production issue occurs, Observability Owner notifies the on-call and Release Manager to trigger the incident playbook; PM and Sponsor Liaison are informed depending on impact.

---

## How to add these personas to process docs

Add a new subsection to docs/octoacme-roles-and-personas.md titled "Additional Personas" (or similar). For each role, include the Role Summary, Responsibilities, Interactions, and Expected Artifacts subheadings as above. Keep entries concise (3–6 bullet responsibilities) and add one example handoff per role where appropriate.
