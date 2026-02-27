# Change Log Template

Use this template to record approved changes to project scope, schedule, resources, or process. Owned by the **Change Control Coordinator**; reviewed by the Project Manager and relevant leads.

---

## Change Log

| ID | Date Raised | Raised By | Description | Category | Impact | Priority | Status | Approved By | Approved Date | Notes |
|----|-------------|-----------|-------------|----------|--------|----------|--------|-------------|---------------|-------|
| CHG-001 | YYYY-MM-DD | _Name_ | _Example: Add new API endpoint for partner integration_ | Scope | Med | High | Approved | _PM Name_ | YYYY-MM-DD | Requires 3-day schedule adjustment |
| CHG-002 | YYYY-MM-DD | _Name_ | _Example: Delay sprint review by 2 days due to holiday_ | Schedule | Low | Low | Approved | _PM Name_ | YYYY-MM-DD | Team notified via Slack |

---

## Change Categories

- **Scope** — additions, removals, or modifications to deliverables
- **Schedule** — changes to milestones, deadlines, or sprint dates
- **Resource** — changes to team composition, assignments, or budget
- **Process** — changes to workflows, tooling, or standards
- **Technical** — architectural or implementation decisions that deviate from the approved plan

---

## Change Request Process

1. **Raise** — any team member submits a change request with description, rationale, and estimated impact.
2. **Assess** — Change Control Coordinator evaluates impact on scope, schedule, and resources with relevant leads.
3. **Decide** — Project Manager (and Product Manager/Sponsor for high-impact changes) approves, rejects, or defers.
4. **Communicate** — Change Control Coordinator updates this log and notifies affected stakeholders.
5. **Implement** — Engineering Lead or relevant owner executes the approved change.
6. **Verify** — QA Lead confirms the change is implemented as approved and quality gates are met.

---

## Status Values

| Status | Meaning |
|--------|---------|
| Pending | Change request raised; under review |
| Approved | Change approved; ready for implementation |
| Rejected | Change not approved; reason documented in Notes |
| Deferred | Change deferred to a future phase/sprint |
| Implemented | Change completed and verified |
| Cancelled | Change withdrawn by the requester |

---

## Related Roles & Documents

- **Change Control Coordinator** — primary owner of this log; see [Roles & Personas](../octoacme-roles-and-personas.md)
- **Project Manager** — approves changes and maintains overall plan alignment
- **QA Lead** — verifies changes meet quality standards
- [Quality Gates Checklist](../checklists/quality-gates-checklist.md)
- [Risks & Communication Process](../octoacme-risks-and-communication.md)
