# OctoAcme — Handoff Checklist

This checklist defines the expected handoffs between project phases and between roles. Use it to ensure accountability is explicit and nothing is lost between transitions.

For full role definitions, see [Roles & Personas](octoacme-roles-and-personas.md).
For a consolidated responsibility overview, see the [RACI Matrix](octoacme-roles-and-personas-raci.md).

---

## Phase 1 → Phase 2: Initiation → Planning

**Handoff owner:** Project Manager  
**Receiving roles:** Project Manager, Product Manager, Business Analyst, QA Lead, Release Manager

### Checklist
- [ ] Project charter / one-pager is approved and accessible in the repo (`docs/`)
- [ ] Stakeholder register is complete and communication cadence is agreed
- [ ] Success metrics are defined and signed off by the Product Manager
- [ ] Initial risk list is documented in the risk register
- [ ] Team roles are confirmed and all personnel are introduced to the project
- [ ] Go/no-go decision for planning is recorded
- [ ] Stakeholder Liaison is briefed and external communication plan is drafted

---

## Phase 2 → Phase 3: Planning → Execution

**Handoff owner:** Project Manager  
**Receiving roles:** Developers, QA Lead, Business Analyst

### Checklist
- [ ] Kickoff meeting held; all delivery team members have attended or reviewed notes
- [ ] Backlog is prioritized and estimated (T-shirt sizing or story points)
- [ ] Acceptance criteria are documented for all items in the first sprint/iteration
- [ ] Definition of Done is agreed and visible to the team
- [ ] Test plan is authored and reviewed by QA Lead
- [ ] Release plan and milestones are documented and shared with the Release Manager
- [ ] Dependencies and integration points are mapped in the project board
- [ ] Development and branching conventions are documented in the repo

---

## Phase 3 → Phase 4: Execution → Risks/Communication (ongoing)

> Note: Risk management and communication are continuous, not a single handoff. This checklist applies at each weekly sync.

**Handoff owner:** Project Manager  
**Receiving roles:** All roles

### Weekly Sync Checklist
- [ ] Risk register is reviewed and updated (owners confirmed for each active risk)
- [ ] Blockers are triaged and escalation path is clear
- [ ] Stakeholder Liaison has sent the weekly external status update
- [ ] QA Lead has reported defect metrics and test progress
- [ ] Scope or priority changes are documented and communicated to relevant parties
- [ ] Action items from the previous sync are reviewed

---

## Phase 3/4 → Phase 5: Execution → Release

**Handoff owner:** Release Manager  
**Receiving roles:** QA Lead, Developers, Project Manager, Product Manager, Stakeholder Liaison

### Pre-Release Checklist
- [ ] All acceptance criteria for the release scope are met and verified by QA
- [ ] QA Lead has provided a formal sign-off (QA sign-off report)
- [ ] CI pipeline is green: tests, linting, and security scans pass
- [ ] Release notes are drafted and reviewed by the Product Manager
- [ ] Rollback plan is documented and shared with the deployment team
- [ ] Deployment window is scheduled and communicated to all stakeholders
- [ ] Smoke test script is ready for post-deploy execution
- [ ] External stakeholders have been notified of the upcoming release (via Stakeholder Liaison)
- [ ] Go/no-go call is held and outcome is recorded

### Deployment Checklist
- [ ] Deploy to staging and run smoke tests; issues resolved or accepted
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy smoke tests; verify key user flows are functional
- [ ] Release announcement sent to stakeholders and support team (Stakeholder Liaison)
- [ ] Release notes published

---

## Phase 5 → Phase 6: Release → Retrospective

**Handoff owner:** Project Manager  
**Receiving roles:** All roles

### Post-Release Checklist
- [ ] Post-release report is documented (incidents, metrics, notes)
- [ ] Any production incidents are triaged and action items are captured
- [ ] Retrospective is scheduled within one week of release
- [ ] Stakeholder Liaison collects external feedback and shares summary with the team
- [ ] QA Lead reviews defect metrics from the release cycle

---

## Cross-Functional Handoffs

### Business Analyst → QA Lead (Requirements to Test Planning)

- [ ] All requirements and acceptance criteria are documented and baselined
- [ ] Ambiguities or open questions are resolved or flagged
- [ ] BA has walked QA Lead through the requirements
- [ ] Traceability matrix (requirements → test cases) is started or referenced

### QA Lead → Release Manager (Test Sign-off to Release)

- [ ] Test execution is complete for the release scope
- [ ] Defect log is reviewed; open defects are accepted or resolved
- [ ] QA sign-off report is provided to the Release Manager
- [ ] Known issues are documented in release notes

### Stakeholder Liaison → Project Manager (External Feedback to Team)

- [ ] External feedback is summarized and shared with the Project Manager
- [ ] High-priority stakeholder concerns are escalated immediately
- [ ] Feedback is logged for the next backlog grooming or planning session

### Release Manager → Project Manager (Post-Deployment)

- [ ] Deployment outcome (success / partial / rollback) is communicated
- [ ] Incidents during deployment are documented and owners assigned
- [ ] Release metrics are shared (e.g., deploy time, rollback frequency)

---

## Handoff Escalation Path

If a handoff is blocked or a dependency is unresolved:

1. The **handoff owner** raises it in the daily standup or via the project channel.
2. The **Project Manager** triages and determines escalation (team-level → Product Lead → Sponsor).
3. The **Stakeholder Liaison** communicates impact to external parties if the block affects external commitments.
4. All decisions and resolutions are documented in the decision log.
