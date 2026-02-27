# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management Documentation. This folder centralizes all process documents that describe how OctoAcme plans, delivers, and continuously improves software projects. Whether you are a new team member looking for orientation or an experienced contributor refreshing your knowledge, start here.

## Process Overview

OctoAcme follows a structured project lifecycle built on four principles: **customer-first** prioritization, **iterative delivery** in small testable increments, **clear ownership** with named Project Manager (PM) and Product Lead (PdM) roles, and **data-informed decisions** guided by measurable outcomes. The lifecycle moves through five phases — Initiation, Planning, Execution & Tracking, Release, and Retrospective — each with defined artifacts, acceptance criteria, and handoff points.

## Roles & Communication

Projects are staffed with well-defined personas: the **PM** coordinates schedules, risk, and communications; the **PdM/Product Lead** owns the roadmap and success metrics; **Developers** implement and test features; **QA/Testing** validates acceptance criteria; and **Stakeholders** provide inputs and approvals. Communication cadences include twice-weekly standups, a weekly PM–PdM sync, monthly stakeholder updates, and ad-hoc escalations recorded in the Risk Register.

## Quality Assurance & Release

Quality is maintained throughout the cycle via a documented testing strategy, CI/security scans on every pull request, and a structured PR review workflow with defined reviewers. Before any production deployment, the team works through a release checklist covering deployment verification, rollback readiness, and post-release monitoring. Learnings from each release feed directly into the Retrospective process to drive continuous improvement.

---

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and lifecycle summary |
| [Project Initiation](octoacme-project-initiation.md) | Problem statement, stakeholders, and high-level timeline |
| [Project Planning](octoacme-project-planning.md) | Scope, milestones, resources, and dependencies |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Build, test, review, and iteration practices |
| [Risks & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, and communication cadences |
| [Release & Deployment](octoacme-release-and-deployment.md) | Deployment process, release checklist, and post-release verification |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retrospective format and action-item tracking |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed responsibilities for each project role |

## Templates & Checklists

Reusable artifacts that operationalize the process documents above. Each artifact is owned by a specific role (see [Roles & Personas](octoacme-roles-and-personas.md)).

| Artifact | Owner | Description |
|----------|-------|-------------|
| [Risk Register Template](templates/risk-register-template.md) | Risk Manager | Track, assess, and mitigate project risks |
| [Quality Gates Checklist](checklists/quality-gates-checklist.md) | QA Lead | Phase-gate sign-off criteria across the lifecycle |
| [Change Log Template](templates/change-log-template.md) | Change Control Coordinator | Log and track all approved project changes |
| [Stakeholder Communication Plan Template](templates/stakeholder-communication-plan-template.md) | Stakeholder Liaison | Plan and track stakeholder communication |

> For project-specific context used by GitHub Copilot Spaces, add process docs to `.copilot/` in your project repository.
