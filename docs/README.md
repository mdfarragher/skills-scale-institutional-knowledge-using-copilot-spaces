# OctoAcme Project Management Docs

This README serves as the entry point for OctoAcme's project management documentation. It provides an overview of our processes and links to all process documents in this folder.

## Overview

OctoAcme follows an end-to-end project lifecycle that moves through five stages: **initiation**, **planning**, **execution and tracking**, **release and deployment**, and **retrospective and continuous improvement**. Each project begins with a lightweight one-pager that captures the problem statement, success metrics, and stakeholder alignment before a go/no-go decision is made to move into planning. During planning, the team breaks work into shippable increments, defines a prioritized backlog with acceptance criteria, establishes a Definition of Done (DoD), and produces a milestone map and release plan. Execution proceeds in iterative sprints, with a structured PR workflow, CI-gated quality checks, and regular demos. Releases follow a standardized checklist covering staging verification, smoke tests, and stakeholder announcements, and every project closes with a structured retrospective to capture learnings and feed them back into future work.

OctoAcme projects are staffed by clearly defined personas: the **Project Manager (PM)** coordinates delivery, schedules, risk, and cross-team communications; the **Product Manager (PdM)** owns the product vision, backlog prioritization, and outcome measurement; **Developers** implement features, maintain test coverage, and participate in design and code review; **QA/Testing** validates quality and acceptance criteria; and **Stakeholders** provide direction, inputs, and approvals at key decision gates.

Communication is structured and predictable across all project phases. The PM and PdM hold a weekly alignment sync, the delivery team runs twice-weekly standups, and stakeholders receive monthly updates. A single source of truth—the project README or release doc—keeps everyone aligned on status. Structured templates standardize weekly status updates (progress, next steps, risks, decisions needed) and incident communications (triage summary, actions taken, timeline, post-incident retrospective). A clear escalation path moves issues from team-level triage → PM → Product Lead → Sponsor, with a dedicated security incident runbook for security-related events.

Quality is enforced throughout the lifecycle. Every backlog item carries explicit acceptance criteria and is subject to the agreed Definition of Done before it is considered complete. The CI pipeline runs automated unit, integration, and security scans on every pull request, and PRs require at least one approval before merging. Pre-release gates mandate that all acceptance criteria are met, CI and security scans pass, release notes are drafted, and a rollback/mitigation plan is in place. Smoke tests run against staging before any production deployment, and a rollback and incident playbook ensures rapid response if a release causes a critical issue.

---

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and high-level lifecycle |
| [Project Initiation](octoacme-project-initiation.md) | Validating and authorizing new work, one-pager template, decision gate |
| [Project Planning](octoacme-project-planning.md) | Backlog creation, estimation, DoD, release plan, and planning checklist |
| [Execution and Tracking](octoacme-execution-and-tracking.md) | Team rhythm, PR workflow, quality practices, and blocker escalation |
| [Risks and Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, communication templates |
| [Release and Deployment](octoacme-release-and-deployment.md) | Release types, deployment checklist, rollback and incident playbook |
| [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retrospective structure, action item tracking, continuous improvement culture |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and communication patterns for each role |
