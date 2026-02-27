# Quality Gates Checklist

Use this checklist before advancing work between key lifecycle phases. Owned by the **Quality Assurance Lead**; sign-off required from the QA Lead and Project Manager before each gate is passed.

---

## Gate 1 — Initiation → Planning

- [ ] Problem statement is clearly defined and approved by Product Manager
- [ ] Acceptance criteria drafted for all in-scope features
- [ ] Definition of Done (DoD) reviewed and agreed by the delivery team
- [ ] Testing strategy documented (unit, integration, E2E, performance as applicable)
- [ ] Known quality risks identified and added to the Risk Register

---

## Gate 2 — Planning → Execution

- [ ] All stories/tasks have acceptance criteria attached
- [ ] Test cases or test plan reviewed by QA Lead
- [ ] CI pipeline configured; all required automated checks enabled
- [ ] Security scanning (SAST/dependency scan) enabled on pull requests
- [ ] Environments (dev, staging) confirmed ready for testing

---

## Gate 3 — Execution → Release Candidate

- [ ] All in-scope features implemented and code-reviewed
- [ ] Unit test coverage meets agreed threshold
- [ ] Integration/E2E tests passing in staging environment
- [ ] No open P0/P1 defects (or exceptions documented and approved)
- [ ] Performance/load tests run (if applicable) with results within acceptable range
- [ ] Security scan results reviewed; critical/high findings resolved or accepted
- [ ] Accessibility checks completed (if applicable)
- [ ] QA Lead sign-off recorded

---

## Gate 4 — Release Candidate → Production

- [ ] Release checklist completed (see [Release & Deployment](../octoacme-release-and-deployment.md))
- [ ] Rollback plan documented and tested
- [ ] Monitoring/alerting verified for new features
- [ ] Stakeholder acceptance / UAT sign-off received (if required)
- [ ] Change request approved via Change Control process (if applicable)
- [ ] Release notes drafted and reviewed
- [ ] Project Manager and QA Lead final sign-off

---

## Gate 5 — Post-Release

- [ ] Production smoke tests passed within agreed window
- [ ] No unexpected errors or alerts in post-release monitoring period
- [ ] Defects found post-release logged and triaged
- [ ] Retrospective scheduled; quality metrics captured

---

## Related Roles & Documents

- **Quality Assurance Lead** — owns this checklist; see [Roles & Personas](../octoacme-roles-and-personas.md)
- **Project Manager** — co-signs gate approvals
- **Change Control Coordinator** — approves production changes at Gate 4
- [Execution & Tracking](../octoacme-execution-and-tracking.md)
- [Release & Deployment](../octoacme-release-and-deployment.md)
