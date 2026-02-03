# OctoAcme Project Management Overview

Welcome to OctoAcme's project management documentation. This guide provides a quick introduction to how we run projects, from initiation through delivery and continuous improvement.

## Project Lifecycle & Core Artifacts

OctoAcme follows a structured yet iterative project lifecycle: Initiation (problem definition and stakeholder alignment), Planning (backlog creation and scope estimation), Execution (building and testing), Release (deployment and verification), and Close (retrospectives and learnings). Each project maintains core artifacts including a Project Charter/One-pager that defines the problem and success metrics, a prioritized backlog with acceptance criteria, a Definition of Done (DoD) to ensure quality standards, a Risk Register to track and mitigate issues, and a Release Plan that maps milestones and timelines. These artifacts serve as the single source of truth throughout the project and enable clear communication across all stakeholders.

## Workflows & Delivery Practices

Teams use project boards (GitHub Projects) with standard columns: Backlog, Ready, In Progress, In Review, QA, and Done. Our pull request workflow emphasizes small PRs (≤400 lines when possible) that include issue links and acceptance criteria, with automated CI checks for tests, linting, and security scans running before review. At least one approval is required before merging. Sprint planning sessions pull items that meet the DoD and respect team capacity, while daily 15-minute standups keep the team synchronized on progress and blockers. Before each release, teams complete a deployment checklist that includes smoke tests in staging, rollback plans, release notes, and post-deployment verifications to ensure production reliability.

## Roles & Communication Cadence

Project teams consist of a Project Manager (PM) who coordinates delivery, schedules, and risk management; a Product Manager (PdM) who defines outcomes and prioritizes the backlog; Developers who implement features and collaborate on design; QA specialists who validate quality and acceptance criteria; and Stakeholders who provide input and approvals. Communication follows a regular cadence: daily standups for the delivery team, weekly syncs between PM and PdM, sprint demos at milestone completion, and monthly stakeholder updates. Escalation follows a clear path—from team-level triage in standups, to PM escalation to Product Lead and dependent teams, up to sponsor-level escalation for business-impacting issues. Security incidents follow dedicated runbooks and notify the Security on-call team.

## QA & Risk Practices

Quality assurance is embedded throughout the development process with unit tests for new logic, integration tests for component interactions, and end-to-end smoke tests for critical flows before release. All CI pipelines include automated security scanning to catch vulnerabilities early. Risks are managed proactively through a Risk Register that captures ID, description, impact, likelihood, owner, mitigation plan, and status—reviewed weekly in team syncs and updated as situations evolve. After each sprint, release, or incident, teams hold retrospectives to identify what went well and what could improve, prioritizing 2–3 actionable items with clear owners and due dates. These action items are tracked in the project backlog, ensuring continuous improvement becomes part of the team's regular workflow rather than a one-time exercise.
