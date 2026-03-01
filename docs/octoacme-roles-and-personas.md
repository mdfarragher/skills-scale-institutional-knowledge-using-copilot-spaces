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

## Technical Lead

### Role Summary
The Technical Lead owns technical decisions, architecture quality, and engineering standards. They bridge the gap between product requirements and technical implementation, guiding Developers while advising the Project Manager on feasibility and risk.

### Responsibilities
- Own architectural decisions and technical standards (coding, testing, tooling)
- Review and approve significant design changes and major PRs
- Identify and communicate technical risks and debt
- Mentor and support Developers in implementation and best practices
- Coordinate with Project Manager and Product Manager on scope, feasibility, and trade-offs

### Goals
- Maintain a scalable, maintainable codebase
- Minimize technical risk and unplanned rework
- Enable Developers to deliver quickly and confidently

### Typical Communication
- Architecture decision records (ADRs) for significant choices
- Technical risk items added to the Risk Register
- Design and code review feedback
- Weekly sync with Project Manager on delivery feasibility

---

## QA Lead / Quality Owner

### Role Summary
The QA Lead defines and owns the test strategy across the project, ensuring quality gates are in place before any release. They coordinate manual and automated QA activities, track defects, and drive resolution to meet release readiness criteria.

### Responsibilities
- Define and maintain the test strategy (unit, integration, end-to-end, exploratory)
- Lead manual and automated QA activities and own the QA column on the project board
- Track bugs, severity classification, and drive resolution with Developers
- Set and enforce quality gates and release readiness criteria
- Report quality status to the Project Manager and Product Manager

### Goals
- Ensure each release meets agreed quality standards before deployment
- Reduce defect escape rate to production
- Build shared quality culture across the team

### Typical Communication
- QA status reports linked to sprint/milestone reviews
- Bug tracking via issues with severity labels
- Go/no-go signal to Release Manager and Project Manager prior to release
- Coordination with Developers for issue reproduction and fixes

---

## UX Designer

### Role Summary
The UX Designer owns user research, interaction design, and usability validation. They translate customer needs into usable, accessible product experiences and ensure design decisions are grounded in evidence.

### Responsibilities
- Conduct user research, usability studies, and synthesize findings
- Create wireframes, prototypes, and design system components
- Collaborate with Product Manager to define experience goals and acceptance criteria
- Work with Developers and QA to ensure correct, accessible implementation of designs
- Advocate for end-user needs throughout the project lifecycle

### Goals
- Deliver intuitive, accessible user experiences
- Ground product decisions in validated user insights
- Reduce rework caused by usability gaps discovered late in development

### Typical Communication
- Design specs and prototype links shared with Developers and QA
- Usability research summaries to Product Manager and Project Manager
- Design review sessions at feature kickoff and before release
- Feedback loops with Support/Customer Advocate on user pain points

---

## Support / Customer Advocate

### Role Summary
The Support/Customer Advocate brings the voice of the customer into the project, surfacing pain points from support channels and ensuring customer experience considerations inform product decisions.

### Responsibilities
- Monitor support channels and aggregate recurring user pain points and feedback
- Represent customer needs in backlog grooming and prioritization discussions
- Contribute to incident reviews with a customer-impact perspective
- Partner with Product Manager and Project Manager on customer experience improvements
- Coordinate with UX Designer to inform research priorities

### Goals
- Ensure customer feedback is visible and actionable in the product roadmap
- Reduce customer-reported defects and friction over time
- Improve customer satisfaction through closed feedback loops

### Typical Communication
- Regular feedback summaries to Product Manager and Project Manager
- Participation in sprint planning and backlog grooming
- Incident review contributions focused on customer impact
- Coordination with UX Designer on research and design priorities

---

## Release Manager

### Role Summary
The Release Manager coordinates release activities, owns the deployment checklist, and drives the go/no-go decision in collaboration with the QA Lead and Project Manager. On small teams, this role may be played by the Project Manager.

### Responsibilities
- Own the release plan, schedule, and deployment checklist
- Coordinate go/no-go decisions with QA Lead, Technical Lead, and Project Manager
- Ensure release notes, rollback plans, and stakeholder communications are prepared
- Drive post-release verification and announce outcomes to stakeholders and Support
- Track and manage release risks and deployment dependencies

### Goals
- Deliver releases on schedule with minimal risk and clear communication
- Ensure all quality gates and pre-release requirements are met before deployment
- Enable fast, confident rollback when needed

### Typical Communication
- Release plan and checklist shared with the full delivery team
- Go/no-go status to Project Manager, QA Lead, and Product Manager
- Release announcements to stakeholders and Support/Customer Advocate
- Post-release summary with incident notes if applicable

---

## Interaction Model / RACI-lite

This section summarizes accountability for key decision areas across all roles. **R** = Responsible, **A** = Accountable, **C** = Consulted, **I** = Informed.

| Decision Area | Tech Lead | QA Lead | UX Designer | Support / Customer Advocate | Release Manager | Developers | Product Manager | Project Manager |
|---|---|---|---|---|---|---|---|---|
| Technical decisions & architecture | **A/R** | C | I | I | I | C | C | I |
| Quality gates & release readiness | C | **A/R** | I | I | C | R | C | I |
| Usability / UX decisions & research | C | C | **A/R** | C | I | C | C | I |
| Customer feedback loops & support signal | I | I | C | **A/R** | I | I | C | C |
| Release coordination & go/no-go | C | C | I | I | **A/R** | I | C | A |
| Backlog prioritization & roadmap | C | C | C | C | I | I | **A/R** | C |
| Project schedule & delivery risk | C | C | I | I | C | I | C | **A/R** |

### Notes
- Where Release Manager role is not filled separately, the **Project Manager** assumes accountability for release coordination.
- The **Technical Lead** has veto authority on technical architecture decisions but must consult the Product Manager on customer-facing trade-offs.
- The **QA Lead** issues the formal go/no-go signal for quality readiness; the **Release Manager** (or Project Manager) makes the final go/no-go call.
- The **UX Designer** and **Support/Customer Advocate** are key inputs to backlog grooming but are not accountable for final prioritization decisions.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Role Assignment Checklist](./octoacme-role-assignment-checklist.md) for a quick-start guide to assigning roles on a new project.

