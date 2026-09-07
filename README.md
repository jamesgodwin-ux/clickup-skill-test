# Onboarding Knowledge Base

Source of truth for the Salesforce to ClickUp onboarding process. These markdown files are read by the "Quorum Onboarding Assistant" skill in Claude, and are the basis for the human-facing training document.

## Files

- **onboarding-training.md** — the training guide: system overview, the end-to-end flow, opportunity tracking, project structure, setting up and working a project, handover, dashboards, access, notifications, edge cases, FAQ, glossary.
- **playbook.md** — the operational playbook: step-by-step checklists per stage (setup, starting, execution, blockers and health, capturing handover, completing handover, project oversight, template version control).
- **appendix-a-automation-requirements.md** — the technical prerequisites for the Teams notifications and Expected End sync, plus a troubleshooting checklist.
- **skill-strategy.md** — how the skill is built, hosted, and maintained (reference for maintainers).

## How this is used

The skill fetches the relevant file from this repo at query time, so updating a file here updates the answers people get, with no need to reinstall the skill.

## Maintaining

1. Edit the relevant markdown file and commit.
2. That is it for content read live by the skill.
3. Regenerate the human training document from `onboarding-training.md` when the process changes.
4. Keep a one-line change log noting what changed, when, and whether it affects the middleware.
