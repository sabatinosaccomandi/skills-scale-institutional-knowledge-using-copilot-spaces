# Risk Register Template

Use this template to identify, assess, and track project risks throughout the lifecycle. Owned by the **Risk Manager**; reviewed weekly by the Project Manager and relevant leads.

---

## Risk Register

| ID | Description | Category | Impact | Likelihood | Risk Score | Owner | Mitigation Plan | Contingency Plan | Status | Last Updated |
|----|-------------|----------|--------|------------|------------|-------|-----------------|------------------|--------|--------------|
| R-001 | _Example: Third-party API deprecation_ | Technical | High | Med | High | Engineering Lead | Evaluate alternative APIs; pin current version | Fall back to internal implementation | Open | YYYY-MM-DD |
| R-002 | _Example: Key team member unavailable during release_ | Resource | Med | Low | Low | Project Manager | Cross-train backup; document handoff steps | Delay release by one sprint | Mitigated | YYYY-MM-DD |

> **Risk Score** = combination of Impact × Likelihood. Use High/Med/Low or a numeric scale (e.g., 1–9) as agreed by the team.

---

## Risk Categories

- **Technical** — architecture, third-party dependencies, infrastructure
- **Resource** — staffing, availability, skill gaps
- **Schedule** — timeline slippage, external dependencies
- **Scope** — requirements creep, unclear acceptance criteria
- **External** — regulatory, market, or vendor changes
- **Security/Compliance** — data handling, access controls, audit requirements

---

## Risk Lifecycle

1. **Identify** — raise new risks at sprint planning, weekly syncs, or ad-hoc as discovered.
2. **Assess** — estimate Impact and Likelihood; assign an owner.
3. **Plan** — document a Mitigation Plan (reduce probability) and Contingency Plan (reduce impact if realized).
4. **Monitor** — review the register at weekly syncs; update Status and Last Updated fields.
5. **Close** — mark risks as Closed once the threat window has passed or the mitigation is complete.

---

## Status Values

| Status | Meaning |
|--------|---------|
| Open | Risk is active and being monitored |
| Mitigated | Mitigation actions are in place; risk is reduced |
| Accepted | Risk is acknowledged; no further action planned |
| Realized | Risk has occurred; contingency plan is active |
| Closed | Risk is no longer applicable |

---

## Related Roles & Documents

- **Risk Manager** — primary owner of this register; see [Roles & Personas](../octoacme-roles-and-personas.md)
- **Project Manager** — reviews and escalates high-priority risks
- **Engineering Lead / Product Manager** — contribute technical and product risk inputs
- [Risks & Communication Process](../octoacme-risks-and-communication.md)
