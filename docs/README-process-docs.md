# OctoAcme — Process Docs Index

## Purpose
- Central index for OctoAcme project & program management process documents.
- Use this page to find, contribute to, and understand governance for process docs.

---

## Frontmatter guidance
Each document in docs/ should include a short frontmatter block at the top with metadata. Example fields:

- owner: @github-username
- status: draft | active | archived
- last_reviewed: YYYY-MM-DD
- tags: [process, planning, release]

Including these fields makes docs easier to discover and maintain.

---

## Core documents
- [octoacme-project-management-overview.md](./octoacme-project-management-overview.md) — high-level lifecycle and roles
- [octoacme-project-initiation.md](./octoacme-project-initiation.md) — initiation checklist and one-pager template
- [octoacme-project-planning.md](./octoacme-project-planning.md) — planning activities and backlog templates
- [octoacme-execution-and-tracking.md](./octoacme-execution-and-tracking.md) — cadence, workflows, checklists
- [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md) — release types and runbooks
- [octoacme-risks-and-communication.md](./octoacme-risks-and-communication.md) — risk register and communication templates
- [octoacme-retrospective-and-continuous-improvement.md](./octoacme-retrospective-and-continuous-improvement.md) — retros and action item tracking
- [octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md) — role descriptions and responsibilities

---

## Brief project management processes summary

OctoAcme organizes work around a clear, stage-based lifecycle to reduce ambiguity and make decision points explicit. Initiation focuses on validating the problem and deciding whether to proceed: teams produce a Project One-pager that captures the problem statement, objective, success metrics, stakeholders, and an initial timeline. When the one-pager and stakeholder alignment are complete, the project moves into planning.

Planning turns the approved initiative into an actionable backlog and release plan. Activities include a kickoff meeting, prioritized backlog items with acceptance criteria, estimates (T-shirt sizing or story points), and a Definition of Done. The planning stage also surfaces dependencies and risks into a lightweight Risk Register so mitigation can be tracked during execution.

Execution emphasizes iterative delivery, small reviews, and automated quality gates. Teams use a project board (Backlog → Ready → In Progress → In Review → QA → Done) and follow PR conventions that encourage small, reviewable changes (aim for <= 400 lines), include issue links and acceptance criteria in PRs, and run CI/lint/security checks before requesting review. QA is a mix of unit, integration, and targeted end-to-end smoke tests; manual QA is used when necessary for acceptance.

Release and continuous improvement complete the cycle: releases follow a checklist (pre-release checks, staged smoke tests, deployment automation when possible, and post-deploy verification) and include a documented rollback/incident playbook. Retrospectives capture what went well, what to improve, and concrete action items with owners and due dates so the team can measure the impact of improvements over time.

---

## How to contribute
1. Open an issue using .github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml (or reference this README) describing the change.
2. Create a branch named `docs/<slug>-<github>-YYYYMMDD` and include the issue number in your PR description.
3. Update or add frontmatter (owner, status, last_reviewed, tags) in the changed files.
4. Assign the doc owner as reviewer and request stakeholder signoff for major changes.

---

## Acceptance criteria for updates
- Content aligns with existing process docs
- Update improves clarity or closes a documented gap
- Proposed content has been reviewed with stakeholders when required

---

_Last updated: 2026-10-18_
