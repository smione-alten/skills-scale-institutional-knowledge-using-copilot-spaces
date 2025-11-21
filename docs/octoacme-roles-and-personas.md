# OctoAcme Roles and Personas

This document defines project roles and personas used across OctoAcme projects. It augments existing role descriptions with additional personas that clarify responsibilities, decision authority, collaboration patterns, and escalation paths. For each role we include: a short summary, core responsibilities, interactions with existing roles, and example scenarios.

## How to use this page
- Use the "Role Template" when adding or changing a role (see docs/templates/role-persona-template.md).
- Use the onboarding checklist to confirm role-fit and responsibilities are communicated (see docs/checklists/role-onboarding-checklist.md).
- Each role entry indicates primary collaborators and typical handoffs.

---

## Existing core roles (summary)
- Project Manager (PM) — Coordinates scope, schedule, resources, and stakeholder communication.
- Product Owner (PO) — Defines product priorities and acceptance criteria; represents business needs.
- Development Lead / Tech Lead — Oversees technical design and implementation.
- Developer — Implements features and fixes.
- Release Manager — Coordinates deployments and release windows.

---

## Proposed additional roles and personas

### Quality Assurance Lead
Summary: Ensures the quality of deliverables through test strategy, test planning, and quality metrics.
Responsibilities:
- Define and maintain QA strategy and test plans.
- Author/maintain acceptance and integration test suites.
- Coordinate test environments and release testing.
- Track quality metrics (defect density, test coverage, test pass rate).
Interactions:
- Works with Development Lead to ensure testability and assign test automation tasks.
- Coordinates with PM to schedule test windows and gating criteria.
- Validates acceptance criteria provided by the Product Owner.
Example scenario: Before a major release, QA Lead runs regression and acceptance suites, raises issues and verifies fixes.

### Change Manager
Summary: Manages scope and process-level change control to reduce disruption.
Responsibilities:
- Receive, triage, and assess change requests.
- Coordinate impact analysis (schedule, cost, risk) with PM and Tech Lead.
- Author change records and track approvals.
- Facilitate communication and rollout plans for approved changes.
Interactions:
- Works with Project Manager and Release Manager to schedule changes.
- Notifies Stakeholders and Product Owner of approved changes and impacts.
Example scenario: When a high-priority scope change is requested mid-sprint, Change Manager facilitates a rapid impact assessment and approval workflow.

### Project Stakeholder
Summary: Represents a business, user, or third-party interest; provides priorities and acceptance.
Responsibilities:
- Provide business context and priorities.
- Review and accept major milestones and deliverables.
- Participate in steering calls and reviews.
Interactions:
- Works with Product Owner to prioritize features.
- Escalates business-level concerns to the Project Manager when risks appear.
Example scenario: Stakeholder signs off on pilot release criteria and provides post-release feedback.

### Agile Coach
Summary: Guides teams on Agile practices, helps improve iterations, and facilitates continuous improvement.
Responsibilities:
- Onboard teams to Agile ceremonies and practices.
- Coach Scrum Masters/Team Leads on facilitation and metrics.
- Run workshops and retrospectives focused on team health and delivery improvement.
Interactions:
- Partners with PM and Development Lead to remove process impediments.
- Supports Product Owner in backlog refinement and prioritization techniques.
Example scenario: Coach runs a series of retrospectives to address recurring sprint carryover issues.

### DevOps Engineer
Summary: Ensures reliable CI/CD, deployment automation, and infrastructure stability.
Responsibilities:
- Build and maintain CI/CD pipelines, deployment scripts, and infrastructure-as-code.
- Support incident response and post-mortem actions.
- Automate observability and alerting for production systems.
Interactions:
- Works closely with Development Lead and Release Manager for safe releases.
- Collaborates with QA Lead to run automated tests in pipelines.
Example scenario: DevOps Engineer adds automated canary deployment and rollout verification for a service.

---

## Interaction guidance & collaboration patterns
- Handoffs (example): PO defines acceptance criteria → Developer implements → QA Lead validates → Release Manager schedules deployment → Stakeholders accept.
- Escalation: If a cross-cutting risk is identified (schedule, security, regulatory), the PM escalates to Steering and notifies Stakeholders and Change Manager.
- RACI example (high-level):
  - Requirements: Responsible = PO, Accountable = Stakeholder, Consulted = PM, DevLead; Informed = Team
  - Release Approval: Responsible = Release Manager, Accountable = PM, Consulted = DevOps, QA Lead; Informed = Stakeholders

---

## Acceptance criteria for role additions
- Content aligns with existing process docs.
- Each role includes responsibilities and interaction examples.
- Document reviewed with core stakeholders before merging.

Refer to: docs/templates/role-persona-template.md and docs/checklists/role-onboarding-checklist.md for artifacts to maintain consistency.