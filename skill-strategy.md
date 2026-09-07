# Onboarding Assistant Skill: Build & Maintenance Strategy

A short strategy for turning the onboarding training content into a Claude skill (and later a plugin) that the team can query while working in ClickUp.

## What we are building

A "Quorum Onboarding Assistant" that anyone in Claude can ask about the Salesforce to ClickUp onboarding process. Two stages:

1. **Skill (stage 1).** Answers questions from our written process, for example "how do I set up the Teams notification?", "what has to be filled in before handover?", "why did my notification not fire?".
2. **Plugin (stage 2).** The skill plus the ClickUp connector, packaged for one click install. It can both explain and query live, for example "which of my projects are Yellow or Red?" or "show me summary tasks ready for handover but missing H_Notes."

## Source of truth: pick one, generate the rest

The single biggest maintenance risk is having the Word doc, the skill's copy, and a ClickUp Doc all drift apart. Choose one canonical source, and produce everything else from it.

Recommended canonical source: **Markdown in a Git repo.** It gives version history, review before changes go live, and clean rollback. From that markdown we generate the Word training doc for humans and the skill's reference files for Claude.

Alternative canonical source: a **ClickUp Doc** in the Onboarding Templates space (next to the existing Template Version Control doc). The skill reads it live, so edits appear immediately with no re-release. Lower ceremony, but no review step and it depends on the doc being reachable.

## Where to host the source docs

- **Git repo (recommended for the skill itself).** One repo holds the skill folder and the canonical markdown. GitHub, Azure DevOps, or wherever the team already keeps code. This is also where versioning and review happen.
- **ClickUp Doc (recommended for the volatile content).** Keep the parts you tune often (automation quirks, edge cases) as a ClickUp Doc the skill reads live, so those stay current without a release.
- **Not the Word .docx.** The Word file is a human deliverable, not a source the skill reads. Treat it as an output, not the master.

## Skill structure

A skill is just a folder:

- `SKILL.md`: the instructions, plus the description that tells Claude when to use it (the triggers, for example "onboarding", "ClickUp handover", "why did my notification fail").
- `references/`: the reference content as markdown, for example `flow.md`, `setup.md`, `handover.md`, `notifications.md`, `troubleshooting.md`, `glossary.md`.
- Optional images (the flow diagram) if you want it to show visuals.

## What to bundle vs read live

- **Bundle (stable, rarely changes):** the end-to-end flow, roles, project structure, glossary, how handover works. These make the skill useful even with no live fetch.
- **Read live (volatile, tuned often):** automation prerequisites and troubleshooting, edge cases, anything still being refined during UAT. Point these at the ClickUp Doc so they are always current.

## Adding live ClickUp queries (the plugin stage)

Bundle the ClickUp connector with the skill so it can answer from live data, not just explain. Scope it to the Onboarding Projects space. Typical questions it could then answer: project health across the portfolio, projects that are blocked or idle, summary tasks missing handover notes, what is due this week.

## Maintenance and versioning workflow

1. Make the change in the canonical source (markdown in the repo, or the ClickUp Doc for live content).
2. If bundled: regenerate the skill's reference files, bump the version, and republish the skill or plugin.
3. If live: no republish needed for content read from the ClickUp Doc.
4. Regenerate the Word training doc from the same source so the human copy stays in step.
5. Announce the version to the team so they update the plugin.

Keep a one line change log (the existing Template Version Control doc is a good home) noting what changed, when, and whether it affects the middleware.

## Recommended approach for us

Given we are a ClickUp shop and want low maintenance:

1. Canonical process text lives as markdown in a small Git repo, which also holds the skill folder.
2. The skill bundles the stable structure so it always works.
3. The skill reads a ClickUp Doc live for the volatile parts, so day to day tuning needs no release.
4. Ship stage 1 (skill) first, validate it with a few onboarders, then add the ClickUp connector to make it a plugin.
5. Version through the repo; keep the change log in ClickUp.

## First steps

1. Decide the canonical source (repo markdown is recommended).
2. Convert the training doc, playbook, and Appendix A into the `references/` markdown set.
3. Write `SKILL.md` with clear triggers and pointers to the reference files and the live ClickUp Doc.
4. Test it with real questions from a new onboarder.
5. Once it feels useful, wrap it as a plugin with the ClickUp connector and roll it out.
