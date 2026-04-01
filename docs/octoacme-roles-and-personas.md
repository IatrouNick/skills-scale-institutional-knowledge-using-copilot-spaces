# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

For a visual overview of who does what across activities and phases, see:
- [RACI Matrix](octoacme-roles-and-personas-raci.md) — responsibility assignments for core activities
- [Handoff Checklist](octoacme-handoff-checklist.md) — phase-to-phase and cross-functional handoff guide

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

### Key Artifacts
- Source code and pull requests
- Unit and integration tests
- Technical design documents

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Provide technical feasibility input |
| Planning | Estimate effort, identify dependencies |
| Execution/Tracking | Implement features, run tests, raise blockers |
| Risks/Communication | Flag technical risks in standups and risk register |
| Release/Deployment | Support deployment, troubleshoot production issues |
| Retro/Improvement | Contribute retrospective items; implement improvement actions |

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Key Artifacts
- Product roadmap
- Prioritized backlog with acceptance criteria
- Success metrics dashboard

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Define problem statement and success metrics; champion initiative |
| Planning | Prioritize backlog; approve Definition of Done |
| Execution/Tracking | Validate deliverables; adjust priorities as needed |
| Risks/Communication | Review risks that affect product goals; approve scope changes |
| Release/Deployment | Approve release readiness; review release notes |
| Retro/Improvement | Assess outcome metrics; feed learnings into roadmap |

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

### Key Artifacts
- Project charter / one-pager
- Risk register
- Status reports and decision logs
- Meeting notes

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Author or review project charter; confirm stakeholder list |
| Planning | Drive kickoff; own release timeline and milestone map |
| Execution/Tracking | Run standups and weekly syncs; update risk register; escalate blockers |
| Risks/Communication | Own stakeholder communication cadence; manage escalations |
| Release/Deployment | Coordinate deployment window; confirm signoffs; announce release |
| Retro/Improvement | Facilitate retrospective; track action items to closure |

---

## Business Analyst (BA)

### Role Summary
Business Analysts bridge the gap between business needs and technical delivery. They gather, clarify, and document requirements to ensure the team builds the right thing.

### Responsibilities
- Gather and document requirements from stakeholders
- Translate business needs into clear, testable acceptance criteria
- Facilitate requirement walkthroughs and clarification sessions
- Validate that delivered features meet stated requirements
- Identify scope gaps and flag conflicting requirements early

### Key Artifacts
- Requirements documentation / user stories
- Acceptance criteria per backlog item
- Process flow diagrams
- Traceability matrix (requirements → deliverables)

### Goals
- Ensure shared understanding of what needs to be built
- Reduce rework caused by misunderstood requirements
- Bridge communication between non-technical stakeholders and the delivery team

### Typical Communication
- Requirement review sessions with Product Manager and Developers
- Clarification threads on backlog items
- Sign-off meetings with stakeholders before development begins

### Interaction with Existing Roles
- **Project Manager:** Provides scoped requirements for planning and flags scope creep risks.
- **Product Manager:** Refines and validates product intent against stakeholder needs.
- **Developers:** Clarifies acceptance criteria and answers implementation questions.
- **QA Lead:** Shares requirements and acceptance criteria to inform test planning.
- **Stakeholder Liaison:** Coordinates external feedback sessions and requirement reviews.

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Assist with problem statement; identify key stakeholders and information needs |
| Planning | Author detailed requirements and acceptance criteria; review backlog items |
| Execution/Tracking | Answer clarification questions; validate work-in-progress against requirements |
| Risks/Communication | Flag scope or requirements risks; document decisions and changes |
| Release/Deployment | Verify release notes accurately reflect delivered requirements |
| Retro/Improvement | Capture requirements-related learnings; improve elicitation process |

---

## QA Lead

### Role Summary
The QA Lead owns quality standards across the project. They plan and coordinate testing activities, track defect resolution, and ensure that acceptance criteria are validated before release.

### Responsibilities
- Define and communicate quality standards and testing strategy
- Plan and execute testing cycles (functional, regression, integration, UAT)
- Track, triage, and coordinate resolution of defects
- Maintain a test plan and test case repository
- Ensure the Definition of Done includes adequate quality gates
- Support and coach team members on testing practices

### Key Artifacts
- Test plan and test strategy document
- Test case suite
- Defect log / bug tracker
- QA sign-off report

### Goals
- Prevent defects from reaching production
- Provide confidence in release readiness
- Foster a quality culture across the team

### Typical Communication
- Sprint planning to align on test scope
- Defect triage meetings with Developers and Product Manager
- QA status updates in weekly delivery sync
- Go/no-go sign-off before release

### Interaction with Existing Roles
- **Developers:** Reviews implementation for testability; pairs on test automation; coordinates defect fixes.
- **Business Analyst:** Uses requirements and acceptance criteria as the basis for test cases.
- **Product Manager:** Escalates quality metrics and seeks clarification on acceptance criteria.
- **Project Manager:** Reports QA status and risks; flags blockers that affect the release timeline.
- **Release Manager:** Provides QA sign-off and readiness confirmation before deployment.

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Review high-level requirements for testability; estimate QA effort |
| Planning | Author test plan; ensure DoD includes quality gates |
| Execution/Tracking | Execute test cycles; log and track defects; update QA status |
| Risks/Communication | Report quality risks; flag untested areas that could delay release |
| Release/Deployment | Provide QA sign-off; execute smoke tests post-deploy |
| Retro/Improvement | Review defect trends; propose process improvements to reduce rework |

---

## Release Manager

### Role Summary
Release Managers own the end-to-end release process. They ensure that all pre-release conditions are met, coordinate deployment activities, and manage the communication of releases to stakeholders.

### Responsibilities
- Develop and maintain release plans and deployment schedules
- Coordinate pre-release sign-offs across QA, Product, and engineering
- Manage deployment activities and communicate status to stakeholders
- Ensure rollback and incident response plans are in place before deploying
- Maintain release notes and post-release reports
- Own the release calendar and coordinate with dependent teams

### Key Artifacts
- Release plan and deployment schedule
- Release checklist (pre-deploy, deploy, post-deploy)
- Release notes
- Rollback and incident response plan
- Post-release report

### Goals
- Ship features reliably with minimal production incidents
- Ensure all stakeholders are informed before, during, and after releases
- Maintain a clear audit trail of deployment activities

### Typical Communication
- Release planning meetings with PM, QA Lead, and Developers
- Pre-release go/no-go calls
- Release announcements to stakeholders and support teams

### Interaction with Existing Roles
- **Project Manager:** Aligns deployment window with project schedule; escalates release risks.
- **QA Lead:** Receives QA sign-off and confirms all test gates are passed before deploying.
- **Developers:** Coordinates deployment steps and troubleshoots deployment issues.
- **Product Manager:** Obtains product sign-off on release scope and release notes.
- **Stakeholder Liaison:** Coordinates release communication to external stakeholders.

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Flag deployment constraints or environment availability early |
| Planning | Draft release plan; define release milestones and freeze dates |
| Execution/Tracking | Monitor release readiness; maintain release checklist |
| Risks/Communication | Identify deployment risks; maintain rollback plan |
| Release/Deployment | Own deployment execution; coordinate go/no-go; publish release notes |
| Retro/Improvement | Review deployment metrics; improve release process based on incidents |

---

## Stakeholder Liaison

### Role Summary
The Stakeholder Liaison is the single point of contact between the project team and external stakeholders (e.g., customers, partners, executive leadership, regulatory bodies). They ensure stakeholders receive timely, consistent information and that their feedback reaches the delivery team.

### Responsibilities
- Serve as the primary contact for external stakeholder inquiries and feedback
- Relay project updates and decisions to external parties in a timely manner
- Represent external stakeholder interests in project discussions
- Coordinate stakeholder reviews, demos, and approval sessions
- Manage stakeholder expectations around timeline, scope, and risk
- Escalate critical external concerns to the Project Manager

### Key Artifacts
- Stakeholder register (list, contact info, communication preferences)
- External communication log
- Stakeholder feedback summaries
- Meeting notes from stakeholder reviews

### Goals
- Maintain stakeholder trust and engagement throughout the project
- Ensure the delivery team has a clear view of external priorities and concerns
- Reduce noise by centralizing and filtering external communications

### Typical Communication
- Regular updates to stakeholder groups (cadence agreed at initiation)
- Ad-hoc responses to stakeholder inquiries
- Coordination calls ahead of major demos, releases, and announcements

### Interaction with Existing Roles
- **Project Manager:** Shares external feedback and escalations; aligns on communication content and cadence.
- **Product Manager:** Relays customer or partner insights that influence product priorities.
- **Business Analyst:** Facilitates requirements sessions with external stakeholders.
- **Release Manager:** Coordinates release announcements with external audiences.
- **Developers:** Arranges stakeholder demos and gathers technical clarification questions from external parties.

### Phase Involvement
| Phase | Involvement |
|---|---|
| Initiation | Build and validate stakeholder register; establish communication cadence |
| Planning | Coordinate stakeholder input sessions; confirm external dependencies |
| Execution/Tracking | Provide regular status updates; relay feedback from stakeholders |
| Risks/Communication | Communicate risks and changes to external stakeholders promptly |
| Release/Deployment | Coordinate external announcements; manage stakeholder expectations at release |
| Retro/Improvement | Collect stakeholder satisfaction feedback; share insights with the team |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See the [RACI Matrix](octoacme-roles-and-personas-raci.md) for a consolidated view of who owns which activities.
- See the [Handoff Checklist](octoacme-handoff-checklist.md) for handoff expectations between phases and roles.

