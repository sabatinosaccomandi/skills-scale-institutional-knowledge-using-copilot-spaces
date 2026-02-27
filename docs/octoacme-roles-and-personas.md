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

## Engineering Lead

### Role Summary
Engineering Leads own the technical direction of a project. They guide architecture decisions, coordinate development work, and serve as the primary technical voice in cross-functional conversations.

### Responsibilities
- Define and communicate technical architecture and standards
- Lead design reviews and architectural decision records (ADRs)
- Identify and escalate technical risks to the Project Manager and Risk Manager
- Coordinate developer capacity and task assignments
- Ensure code quality standards and CI practices are followed

### Goals
- Deliver a maintainable, scalable technical solution
- Reduce technical debt and unplanned rework
- Enable developers to move quickly with confidence

### Typical Communication
- Daily standups and sprint planning with developers
- Weekly syncs with Project Manager and Product Manager
- Technical design docs and ADRs in the project repo

---

## Risk Manager

### Role Summary
The Risk Manager proactively identifies, documents, and tracks project risks. They coordinate mitigation and escalation with project leads and stakeholders to keep exposure within acceptable bounds.

### When They Are Needed
- Active from planning through project close; most critical during planning and execution phases
- Engaged when new vendors, integrations, or significant scope changes are introduced

### Responsibilities
- Maintain and update the [Risk Register](templates/risk-register-template.md) throughout the project lifecycle
- Facilitate risk identification sessions during planning and sprint reviews
- Assess impact and likelihood for each risk; assign owners
- Track mitigation actions and confirm completion
- Escalate high-priority risks to the Project Manager and relevant stakeholders
- Archive closed risks with documented outcomes

### Key Interactions
- **Project Manager** — escalates high risks; aligns on mitigation prioritization
- **Engineering Lead** — identifies and owns technical risks
- **Product Manager** — surfaces scope and business risks
- **Change Control Coordinator** — flags risks introduced by approved changes

### Lifecycle Touchpoints
| Phase | Activities |
|-------|-----------|
| Initiation | Initial risk brainstorm; seed the Risk Register |
| Planning | Full risk assessment; assign owners and mitigation plans |
| Execution | Weekly risk review; update statuses; raise new risks |
| Release | Confirm release-blocking risks are mitigated or accepted |
| Retrospective | Review realized risks; capture learnings for future registers |

### Outputs / Artifacts
- [Risk Register](templates/risk-register-template.md) _(owned)_
- Risk summary section of weekly status reports

---

## Quality Assurance Lead

### Role Summary
The Quality Assurance (QA) Lead ensures quality standards are defined, communicated, and tracked throughout delivery. They collaborate with engineering and product management to validate that each increment meets acceptance criteria before advancing to the next phase.

### When They Are Needed
- Active from planning through post-release monitoring
- Critical at every phase transition (quality gates)

### Responsibilities
- Define the testing strategy (unit, integration, E2E, performance, accessibility) at project start
- Maintain and enforce the [Quality Gates Checklist](checklists/quality-gates-checklist.md)
- Review and approve test plans and acceptance criteria with developers and Product Manager
- Monitor CI/CD pipeline results and raise failures with the Engineering Lead
- Track and triage defects; escalate P0/P1 issues to the Project Manager
- Provide sign-off before each quality gate is passed
- Capture quality metrics for retrospective review

### Key Interactions
- **Engineering Lead** — aligns on test coverage standards and CI configuration
- **Product Manager** — confirms acceptance criteria and validates UAT outcomes
- **Project Manager** — reports quality status; co-signs gate approvals
- **Change Control Coordinator** — verifies that approved changes meet quality requirements

### Lifecycle Touchpoints
| Phase | Activities |
|-------|-----------|
| Initiation | Review scope for testability; flag quality risks |
| Planning | Define testing strategy; establish DoD; gate criteria agreed |
| Execution | Review PRs for test coverage; monitor CI; triage defects |
| Release | Final gate sign-off; production smoke test plan ready |
| Retrospective | Analyze defect trends; propose process improvements |

### Outputs / Artifacts
- Testing strategy document _(owned)_
- [Quality Gates Checklist](checklists/quality-gates-checklist.md) _(owned)_
- Defect triage log _(contributed)_

---

## Change Control Coordinator

### Role Summary
The Change Control Coordinator is the central point for managing requested changes to project scope, schedule, resources, or process. They document decisions, disseminate updates, and track follow-through to ensure changes are implemented as approved.

### When They Are Needed
- Any time a change request is raised that affects the approved project baseline
- Particularly important during execution and release phases when change frequency is highest

### Responsibilities
- Receive, log, and triage all change requests in the [Change Log](templates/change-log-template.md)
- Coordinate impact assessments with the Engineering Lead, QA Lead, and Risk Manager
- Present change requests to the Project Manager (and sponsor for high-impact changes) for decision
- Communicate approved, rejected, or deferred decisions to all affected parties
- Track implementation of approved changes and confirm completion with the relevant owner
- Maintain an audit trail of all change decisions

### Key Interactions
- **Project Manager** — primary decision-maker on change approvals
- **Engineering Lead** — assesses technical impact of proposed changes
- **QA Lead** — confirms quality gates are met post-change
- **Risk Manager** — flags risks introduced by changes
- **Stakeholder Liaison** — coordinates external stakeholder notifications for approved changes

### Lifecycle Touchpoints
| Phase | Activities |
|-------|-----------|
| Initiation | Establish change control process; define approval thresholds |
| Planning | Baseline scope, schedule, and resources; document in Change Log |
| Execution | Process and communicate change requests as they arise |
| Release | Approve or reject last-minute change requests; update release notes |
| Retrospective | Review change volume and patterns; identify process improvements |

### Outputs / Artifacts
- [Change Log](templates/change-log-template.md) _(owned)_
- Change decision communications _(owned)_

---

## Stakeholder Liaison

### Role Summary
The Stakeholder Liaison maintains active communication with key external stakeholders. They gather feedback, communicate updates, and ensure ongoing alignment between stakeholder expectations and project objectives.

### When They Are Needed
- Active from initiation through project close; critical during release and major milestone events
- Essential when the project involves external partners, customers, or executive sponsors

### Responsibilities
- Build and maintain the [Stakeholder Communication Plan](templates/stakeholder-communication-plan-template.md)
- Identify all stakeholder groups, their communication needs, and preferred channels
- Send scheduled status updates and milestone announcements
- Gather and log stakeholder feedback; triage with the Product Manager and Project Manager
- Coordinate UAT and acceptance activities with relevant stakeholders
- Escalate stakeholder concerns or blockers to the Project Manager promptly
- Ensure release communications (release notes, announcements) reach all relevant parties

### Key Interactions
- **Project Manager** — aligns on escalation decisions and stakeholder messaging
- **Product Manager** — coordinates on roadmap updates and customer-facing communication
- **Change Control Coordinator** — notifies stakeholders of approved changes that affect them
- **Engineering Lead** — gathers technical summaries for stakeholder-ready communication

### Lifecycle Touchpoints
| Phase | Activities |
|-------|-----------|
| Initiation | Populate stakeholder registry; schedule kickoff meeting |
| Planning | Share timeline and milestones; confirm communication cadences |
| Execution | Send bi-weekly (or agreed) status updates; log feedback |
| Release | Distribute release announcement and notes to all stakeholder groups |
| Retrospective | Share outcomes and learnings with stakeholders as appropriate |

### Outputs / Artifacts
- [Stakeholder Communication Plan](templates/stakeholder-communication-plan-template.md) _(owned)_
- Stakeholder registry _(owned)_
- Milestone announcements and release communications _(owned)_

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

## Supporting Templates & Checklists

The following artifacts operationalize the roles defined above and are maintained under `docs/`:

| Artifact | Owner | Description |
|----------|-------|-------------|
| [Risk Register Template](templates/risk-register-template.md) | Risk Manager | Track, assess, and mitigate project risks |
| [Quality Gates Checklist](checklists/quality-gates-checklist.md) | QA Lead | Phase-gate sign-off criteria across the lifecycle |
| [Change Log Template](templates/change-log-template.md) | Change Control Coordinator | Log and track all approved project changes |
| [Stakeholder Communication Plan Template](templates/stakeholder-communication-plan-template.md) | Stakeholder Liaison | Plan and track stakeholder communication |

