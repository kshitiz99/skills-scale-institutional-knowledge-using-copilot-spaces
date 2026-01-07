# OctoAcme Project Management Framework

Welcome to the OctoAcme project management documentation. This README serves as the entry point for understanding how OctoAcme manages cross-functional projects from initiation through retrospectives.

## Overview

OctoAcme's project management framework is designed to deliver customer value through iterative, data-informed delivery with clear ownership and psychological safety. Our approach emphasizes small, testable increments while maintaining transparency and alignment across all stakeholders.

### Core Principles

- **Customer-first**: Prioritize customer value and usability in every decision
- **Iterative delivery**: Deliver small, testable increments to reduce risk and accelerate feedback
- **Clear ownership**: Each project has a named Project Manager (PM) and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback, learning, and continuous improvement

## Project Lifecycle Workflow

OctoAcme projects follow a structured five-phase lifecycle:

### 1. **Initiation**
- Validate business need and define measurable outcomes
- Identify stakeholders and champions
- Create a Project One-pager with problem statement, goals, and success metrics
- Confirm team availability and initial timeline
- **Decision gate**: Move to planning when success metrics are clear and stakeholders align on priority

### 2. **Planning**
- Conduct kickoff meeting with stakeholders and delivery team
- Break work into prioritized backlog with acceptance criteria
- Estimate scope and define Definition of Done (DoD)
- Identify dependencies, risks, and integration points
- Create release plan and milestone roadmap

### 3. **Execution & Tracking**
- Follow daily standups (15 min) and weekly delivery syncs
- Use project board workflow: Backlog → Ready → In Progress → In Review → QA → Done
- Maintain small PRs (<= 400 lines) with clear issue links and acceptance criteria
- Monitor velocity, burndown, and key success metrics
- Update risk register weekly

### 4. **Release & Deployment**
- Verify all acceptance criteria met and CI passing
- Deploy to staging and run smoke tests
- Execute production deployment with post-deploy verification
- Announce release to stakeholders and support teams
- Have rollback plan ready for incident response

### 5. **Retrospective & Continuous Improvement**
- Conduct retrospective after each sprint, release, or milestone
- Capture "what went well" and "what could be improved"
- Prioritize 2-3 actionable improvements with owners and due dates
- Track action items in project backlog and review in weekly syncs

## Roles & Responsibilities

### Project Manager (PM)
- Coordinates delivery activities, schedules, and risk management
- Facilitates meetings (kickoffs, planning, retrospectives)
- Ensures project documentation and status reporting
- Escalates blockers and manages stakeholder communication
- **Goal**: Deliver projects on time, within scope, with minimal unplanned work

### Product Manager (PdM)
- Defines product vision, problem statements, and success metrics
- Prioritizes roadmap and backlog based on customer and business value
- Validates solutions through user research and metrics
- Collaborates on trade-offs with stakeholders and engineering
- **Goal**: Maximize customer value and ensure product-market fit

### Developers
- Design, build, test, and deliver software components
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Identify technical risks and propose mitigations
- **Goal**: Deliver reliable, maintainable code with high test coverage

### QA/Testing
- Validate quality and acceptance criteria
- Perform manual QA for feature acceptance when needed
- Support integration and end-to-end smoke tests
- Collaborate on test planning and execution

### Stakeholders
- Provide inputs, requirements, and approvals
- Receive regular updates and release announcements
- Support decision-making and prioritization

## Communication Strategies

### Standard Communication Rhythms

- **Daily standups** (15 min): Team-level sync on progress, blockers, dependencies
- **Twice-weekly team standups**: As agreed by delivery team
- **Weekly PM + PdM sync**: Alignment on priorities, risks, and decisions
- **Weekly delivery sync**: Progress updates, demos, and risk reviews
- **Monthly stakeholder updates**: Status, metrics, and roadmap alignment
- **Sprint/milestone demos**: Showcase completed work and gather feedback
- **Ad-hoc escalations**: As needed for critical issues

### Communication Templates

**Weekly Status Update**:
- Progress this week
- Next steps
- Risks & blockers
- Asks / decisions needed

**Incident Communication**:
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident retrospective scheduled

### Escalation Paths
- **Level 1**: Team-level triage in daily standup
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues
- **Security incidents**: Follow security incident runbook and notify Security on-call

## Quality Assurance Practices

### Testing Strategy
- **Unit tests**: For all new logic and components
- **Integration tests**: Where applicable for component interactions
- **End-to-end smoke tests**: For critical flows before each release
- **Security scanning**: Automated in CI pipeline
- **Manual QA**: For feature acceptance when needed

### Pull Request Workflow
- Keep PRs small (<= 400 lines when possible)
- Include issue link and acceptance criteria in PR description
- Run automated tests and linting in CI before requesting review
- Require at least one approval before merging (or team-defined policy)

### Quality Gates
- All acceptance criteria met
- Passing CI and security scans
- Code review approved
- Definition of Done satisfied
- Release notes drafted
- Rollback/mitigation plan documented

### Risk Management
Maintain a Risk Register with:
- ID, Description, Impact, Likelihood
- Owner and Mitigation plan
- Status (Identified → Assessed → Mitigated → Monitored)
- Review risks at weekly syncs and update regularly

## Key Artifacts

Throughout the project lifecycle, OctoAcme teams maintain these key documents:

- **Project Charter / One-pager**: Problem statement, goals, success metrics, stakeholders
- **Roadmap and Release Plan**: Timeline, milestones, and dependencies
- **Sprint/Iteration Backlog**: Prioritized work items with acceptance criteria
- **Acceptance Criteria & Definition of Done**: Clear standards for completion
- **Risk Register**: Active tracking of risks, impacts, and mitigations
- **Retrospective Notes and Action Items**: Learnings and improvement commitments

## How to Use These Docs

- Keep your Project Charter updated in the project repository
- Add process-specific docs into `.copilot/` for Copilot Spaces context
- Reference these process documents when setting up new projects
- Use templates and checklists to ensure consistency
- Adapt processes to fit your team's specific needs while maintaining core principles

---

## Documentation Navigation

Explore the complete OctoAcme project management documentation:

### Core Documentation
- **[Project Management Overview](octoacme-project-management-overview.md)** - Principles, roles, artifacts, and high-level lifecycle

### Roles & Team Structure
- **[Roles and Personas](octoacme-roles-and-personas.md)** - Detailed responsibilities for Developers, Product Managers, and Project Managers

### Process Guides
- **[Project Initiation](octoacme-project-initiation.md)** - Validate ideas, align stakeholders, and create initial plans
- **[Project Planning](octoacme-project-planning.md)** - Turn approved initiatives into actionable backlogs and release plans
- **[Execution and Tracking](octoacme-execution-and-tracking.md)** - Day-to-day workflows, team rhythm, and progress tracking
- **[Risks and Communication](octoacme-risks-and-communication.md)** - Risk management, stakeholder updates, and escalation paths
- **[Release and Deployment](octoacme-release-and-deployment.md)** - Pre-release requirements, deployment checklists, and rollback procedures
- **[Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)** - Capture learnings and drive actionable improvements

---

## Getting Started

**New to OctoAcme?** Start with the [Project Management Overview](octoacme-project-management-overview.md) to understand our core principles and approach.

**Starting a new project?** Follow the [Project Initiation](octoacme-project-initiation.md) guide to create your Project One-pager.

**Looking for specific guidance?** Use the navigation links above to jump to the relevant process document.

**Questions or feedback?** Reach out to your Project Manager or Product Lead for guidance on applying these processes to your specific project needs.
