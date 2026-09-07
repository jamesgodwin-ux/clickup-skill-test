# Appendix A — Automation Requirements & Troubleshooting

*Why a notification might not fire*

The Teams notifications and the Expected End sync depend on a few conditions being in place on the triggering task and its Project Summary task. When a notification does not arrive, it is almost always one of the items below.

## Shared prerequisites (all automations)

- **Matching tag.** The triggering task and its Project Summary task must share at least one identical tag. This is how the flow locates which summary task belongs to the project. Don't strip the application tags off tasks.
- **Project Summary list.** A list whose name contains "project summary" (case-insensitive) must exist under the same folder as the triggering task.

## Teams notification routing (the `type` parameter)

- `test` sends immediate success (no downstream dependencies).
- `health`, `app_started`, `app_completed`, `app_blocked`, `app_unblocked`, `app_handoverFailed` route to the summary branch.
- `task_started`, `task_completed`, `task_blocked`, `task_unblocked` route to the task branch.
- Anything else returns `401 Unauthorized` and nothing is sent.

## Resolving the Teams channel

- The Project Summary task must have the **Team Notify** custom field populated with a valid Teams deep link, containing both `groupId=` and a `/channel/{id}/` segment. A malformed link means the channel cannot be resolved.

## Field requirements by notification type

- **Health / blocker notifications.** Project Health and/or Blockers dropdown fields should be set on the task, or the card falls back to "No health set" / "No blocker set."
- **Task start / complete notifications.** Notify Start Message / Notify End Message fields are optional but surfaced on the card if present.

## Expected End sync

- The triggering task must have a Due Date set.
- The Project Summary task must have a custom field named exactly "Expected End." The field-ID lookup fails if the name does not match exactly.

## Troubleshooting checklist (if a notification did not fire)

- Is there a list containing "project summary" in the same folder as the task?
- Do the triggering task and its summary task share at least one identical tag?
- Is the Team Notify field a valid Teams link (contains `groupId=` and `/channel/{id}/`)?
- Is the correct `type` value being used for that notification?
- Health/blocker card blank? Confirm Project Health / Blockers are set on the task.
- Expected End not syncing? Confirm the task has a Due Date and the summary field is named exactly "Expected End."
