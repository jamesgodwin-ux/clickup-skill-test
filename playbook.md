# SECTION 1 — APPLICATION PLAYBOOK

## 1\. Application Summary Setup & Ownership

### Purpose

Set up the application correctly so onboarding can begin with **clear
ownership, timeline, and context**.

### Checklist

  - Review Salesforce data populated in the Application Summary Task

  - Confirm Application is relevant (not mistakenly included)

  - Assign yourself as the Application Owner

  - Review and confirm Client Contact Name and Email

  - Review Applications Sold and Applications Existing

  - Review Contract Closed Date and Copy of Contract

  - Review Application Notes and Milestone Details

  - Identify if a Partner is involved

  - Confirm Partner Type and Partner Name (if applicable)

  - Review Integration Setup and Mapping & Matching requirements

  - Review Expected Start and Expected End planning dates. Don’t set
    dates for Actual Start and End. These will be set automatically.

  - Confirm project duration assumptions for planning visibility

  - Assign supporting Onboarders (if required)

  - Set initial Application Health to **Green (On Track)**

  - Create and name the Teams channel for this project

  - Copy the Teams channel link and paste it into the team\_notify\_id
    field

### Guidance

  - This step is about **understanding what was sold**, not starting
    work yet

  - All data here comes from Salesforce and may be **incomplete or
    slightly incorrect**

  - You are responsible for validating and correcting it early

  - If something looks wrong, flag it immediately before proceeding

### Setting Up Teams Channel Notifications

Each application's Start and End notifications post to a Teams channel
set on the Application Summary Task. Set this up once when the
application is created.

1.  In Teams, create (or choose) the channel and name it (e.g.
    “Onboarding – \<Client\>”).

2.  Next to the channel name, click … → **Copy link**.

3.  Paste the link into the **team\_notify\_id** field on the
    Application Summary Task.

4.  Check **Notify on Start** and enter the **Notify Start Message**.

5.  Check **Notify on End** and enter the **Notify End Message**.

### Common Mistakes to Avoid

  - Starting work without reviewing contract or milestones

  - Not assigning ownership clearly

  - Ignoring partner involvement (this causes delays later)

  - Leaving Application Health unset

### Notifications Triggered

  - Assigning users → may trigger internal visibility (ClickUp / Teams)

  - No external/client emails are sent at this stage

# SECTION 2 — STARTING THE APPLICATION

## 2\. Triggering Onboarding2. Triggering Onboarding

### Purpose

Formally start onboarding, so the application moves from planning into
execution, with timelines and tracking activated.

### Checklist

  - Confirm all setup details in Section 1 are complete

  - Set the Application Summary Task status to **In Progress**

  - Set the Due Date based on the length of the actual onboarding. This
    should never be changed once set. This can be aligned with the task
    list seen on the timeline view after the next step that will show
    the estimated end date.

  - Confirm dependency chain is intact across execution tasks

  - Set Start Date on the first execution task

  - Confirm all required onboarders are assigned

  - Identify the first task to begin onboarding

  - Move the first task to **In Progress**

  - Confirm Actual Start Date is populated

  - Review task dependencies (especially if dependent on another
    application like ODA)

### Guidance

  - The **official start trigger** is changing the Application Summary
    Task to **In Progress**

  - This action signals:
    
      - onboarding has begun
    
      - timelines are now active
    
      - ClickUp timeline and Gantt calculations rely on native task
        Start Dates, Durations, and Dependency Relationships.
    
      - The execution task list — not custom date fields — drives
        operational scheduling.
    
      - tracking begins for reporting and dashboards

  - The **first task moved to In Progress** is critical:
    
      - it determines when onboarding started
    
      - this is used to measure delays between kickoff and real work
    
      - Setting the Start Date on the first execution task activates
        downstream scheduling calculations across the dependency chain.
    
      - Once activated, ClickUp automatically calculates future task
        dates using task durations and dependencies.

  - Always ensure:
    
      - dependencies are understood
    
      - no upstream blockers exist before starting

### Common Mistakes to Avoid

  - Starting tasks before setting the Application Summary to In Progress

  - Forgetting to set or validate the Due Date

  - Starting work without checking dependencies (especially
    cross-application dependencies)

  - Starting too early when the client is not ready

### Notifications Triggered

Internal (Teams / ClickUp):

  - Application Onboarding Started (status moved to In Progress)

  - Assigned team members become active on the application

Potential downstream impact:

  - This action contributes to:
    
      - start delay tracking
    
      - capacity tracking
    
      - onboarding timeline metrics

# SECTION 3 — MANAGING EXECUTION

## 3\. Tasks, Dependencies, and Progress3. Tasks, Dependencies, and Progress

### Purpose

Execute onboarding tasks in a structured way while maintaining
visibility, progress tracking, and alignment with dependencies.

### Checklist

  - Work through tasks in the Application List in priority order

  - Ensure each task is assigned to the correct owner

  - Update task statuses as work progresses (Not Started → In Progress →
    Complete)

  - Follow defined task dependencies (do not skip dependent steps)

  - Add notes to tasks where configuration or decisions are made

  - Capture any important client-specific details in tasks

  - Ensure tasks include required details (training content, links,
    references)

  - Monitor milestone progress (e.g. Pre-Test, Training, Go-Live)

  - Keep task estimates and due dates accurate (if adjustments are
    needed)

  - Regularly review progress against the application timeline

  - Do not remove or break dependency relationships between tasks

  - Maintain task durations unless operationally required

### Guidance

  - The Application List contains all execution-level work

  - Tasks represent:
    
      - configuration steps
    
      - training
    
      - setup
    
      - client actions

  - Always treat tasks as:
    
      - source of truth for what was done

<!-- end list -->

  - If something important happens:
    
      - configuration change
    
      - client decision
    
      - Workaround

**it must be recorded in the task**

  - This ensures:
    
      - clean handover to Customer Support
    
      - traceability later

### Dependencies (Important)

  - Some applications depend on others (e.g. ODL depends on ODA)

  - Do not start dependent work unless prerequisite tasks are complete

  - If blocked by another application:
    
      - record blocker (next section)
    
      - do not force progress

  - Dependency relationships are required for accurate Gantt, Timeline,
    and capacity calculations.

  - Removing dependencies or durations may break project scheduling
    visibility.

### Milestones

Milestones drive both:

  - internal tracking

  - client communication

Examples include:

  - Pre-Test Conversion Prep

  - Test Conversion

  - Training

  - Go-Live

Reaching a milestone may trigger:

  - email updates

  - internal notifications

  - reporting updates

### Common Mistakes to Avoid

  - Completing tasks without updating status

  - Skipping dependencies to “move faster”

  - Not documenting configuration decisions

  - Letting tasks sit in “In Progress” without activity

  - Ignoring milestone tracking

### Notifications Triggered

Internal:

  - Task status updates

  - Milestone reached notifications

  - Team visibility updates

External (Email):

  - Milestone updates to stakeholders

  - Progress-related communications (if configured)

# SECTION 4 — BLOCKERS, IDLE STATE, AND RISK MANAGEMENT

## 4\. Managing Issues and Escalation4. Managing Issues and Escalation

### Purpose

Ensure issues are clearly identified, structured, and visible so they
can be resolved quickly and reported accurately.

### Checklist

  - Identify when a task or application is blocked

  - Record the issue in the relevant task (what is blocked and why)

  - Update the Blockers field on the Application Summary Task

  - Select the correct blocker category (Client, Quorum, Partner)

  - Communicate blocker to relevant stakeholders (internal or external)

  - Adjust Application Health if required (Green → Yellow → Red)

  - Monitor blocked items regularly until resolved

  - Update or remove blocker once resolved

  - Identify if lack of activity qualifies as Idle

  - Mark application as Idle if appropriate

  - Continue follow-ups for Idle clients or dependencies

### Guidance

  - Blockers exist at two levels:
    
      - Task level → operational detail
    
      - Application Summary → reporting and visibility

  - The Blockers field must always reflect the current state of the
    application

### Idle State

  - Idle is triggered when there is:
    
      - no meaningful activity
    
      - or ongoing delays from client/partner

  - Idle can be:
    
      - detected automatically (e.g. no activity over time)
    
      - set manually when you know progress has stalled

  - Idle applications should:
    
      - be clearly flagged
    
      - be actively followed up
    
      - be visible in dashboards

  - Idle Status is operationally managed through the dedicated “Idle
    State” ClickUp view and related governance fields.

  - Idle Status may also trigger automated Teams and email notification

### Health Management

Application Health must reflect reality:

  - Green → On track, no issues

  - Yellow → Some risk, manageable delays or blockers

  - Red → At risk, major blockers or delays

Health is:

  - set by the Onboarder

  - guided by blockers, delays, and idle state

### Common Mistakes to Avoid

  - Leaving blockers only in tasks (not reflected in summary)

  - Delaying escalation of client or partner issues

  - Keeping Health as Green when there are clear risks

  - Ignoring Idle signals

### Notifications Triggered

Internal:

  - Blocked tasks visibility in dashboards

  - At-risk applications appear in reporting

  - Idle applications flagged for review

External:

  - Follow-up communications to clients or partners

  - Escalation discussions where required

# SECTION 5 — CAPTURING CONTEXT FOR HANDOVER

## 5\. Capturing the Handover (H\_Notes Template)5. Capturing the Handover (H\_Notes Template)

### Purpose

Capture all relevant onboarding contexts so Customer Support can
confidently take over the client without gaps or rework.

### Checklist

  - Open the standard handover template document

  - Complete the template throughout onboarding, not at the end — update
    it as things happen

  - Capture overall onboarding status and UAT status

  - Capture unique configuration notes and integrations enabled

  - Capture risks, unresolved issues, and client concerns

  - Capture client sentiment, engagement level, and internal champion(s)

  - Capture at-risk indicators / follow-up recommendations and the
    ClickUp project link

  - Add any final notes for the Customer Success team

  - Save the completed template and attach it to the H\_Notes field on
    the Application Summary Task

  - Confirm the latest version is the one attached in H\_Notes (replace
    any older copy)

### Guidance

  - The handover template should be updated throughout onboarding, not
    at the end

  - Think of this as building a handover narrative over time

  - Every time something important happens, ask:
    
      - Will Customer Support need to know this later?
    
      - If yes → capture it in the handover template, then save it as
        the attachment in the H\_Notes field

### What Should Be Captured

Examples of valuable context:

  - Custom configurations or workarounds

  - Integration details and limitations

  - Client expectations or sensitivities

  - Known issues or incomplete areas

  - Training gaps or user readiness

  - Any non-standard implementation decisions

### Why This Matters

  - Customer Support does not have full onboarding context

  - Missing information leads to:
    
      - support tickets
    
      - rework
    
      - poor client experience

This step ensures:

  - Continuity from onboarding → support

### Common Mistakes to Avoid

  - Leaving the handover template until the end

  - Only filling required fields, not meaningful context

  - Forgetting to capture configuration details

  - Not recording unresolved issues

  - Ignoring client sentiment and engagement

### Ownership

  - The assigned Onboarder is responsible for maintaining these fields

  - The onboarding manager may review, but does not own this step

### Notifications Triggered

None directly at this stage

However:

  - The completed H\_Notes attachment is later used by the middleware

  - They directly impact Salesforce records and reporting

# SECTION 6 — COMPLETING THE APPLICATION & TRIGGERING HANDOVER

## 6\. Customer Support Handover6. Customer Support Handover

### Purpose

Finalize onboarding and transfer a complete, accurate record of the
application to Customer Support.

### Checklist

  - Confirm all relevant tasks are complete or appropriately documented

  - Confirm Actual End has been captured correctly

  - Confirm the completed handover template is attached to the H\_Notes
    field (latest version)

  - Perform a final review of the Application Summary Task

  - Check H\_Ready for Handover

### Guidance

The application does not need to be 100% complete

It must be:

  - Clear, documented, and ready for Customer Support to take ownership

Actual End is used for operational KPI reporting and comparison against
the Expected End baseline.

Before checking H\_Ready for Handover, ensure:

  - nothing critical is missing

  - all known issues are documented

  - Customer Support can continue without confusion

### What Happens After You Check “Ready for Handover”

  - A webhook is triggered

  - Middleware collects the H\_Notes handover attachment (and the
    handover flags)

  - Data is pushed into Salesforce

If successful:

  - H\_Handover Captured = true

### Important Rules

Do not check H\_Ready for Handover:

  - if key information is missing

  - if configuration details are incomplete

  - if major risks are undocumented

**You only get one clean handover opportunity**

### Common Mistakes to Avoid

  - Treating this as a checkbox exercise instead of a quality handover

  - Forgetting to document configuration or integration details

  - Leaving unresolved issues undocumented

  - Not attaching the completed handover template to H\_Notes

  - Checking handover too early

### Notifications Triggered

System:

  - Middleware webhook triggered

  - Salesforce updated with onboarding data

Internal:

  - Application marked as handed over

  - Application is ready for project-level completion workflow

### Final Outcome

  - Customer Support receives a complete onboarding record

  - Application is marked as handed over (H\_Handover Captured = true)

  - Reporting and dashboards reflect completion

# SECTION 7 — PROJECT-LEVEL PLAYBOOK

## 7\. Project Oversight & Completion (Manager)7. Project Oversight & Completion (Manager)

### Purpose

Provide oversight across all applications, manage overall project
health, and complete the onboarding lifecycle at project level.

### Checklist

  - Review all Application Summary Tasks for the project

  - Confirm each application has been handed over (H\_Handover Captured
    = true)

  - Identify any applications still in progress or blocked

  - Review Application Health across all applications

  - Set overall Project Health (Green / Yellow / Red)

  - Identify any cross-application risks or dependencies

  - Confirm no outstanding critical blockers remain

  - Ensure all required handovers to Customer Support are complete

  - Perform final review of Project Summary Task fields

  - Confirm project is ready for closure

  - Move project to the “Onboarding Complete" Space in ClickUp

### Guidance

  - Project Health is manually set by the onboarding manager

It should reflect:

  - Overall client onboarding state across all applications
    
      - Consider:
        
          - application health
        
          - Blockers
        
          - idle states
        
          - Delays
        
          - client engagement

### Project Completion Criteria

Project timelines and reporting visibility rely on the integrity of:

  - execution task dependencies

  - task durations

  - native ClickUp scheduling dates

Custom planning fields support forecasting but do not drive scheduling
calculations.

A project is considered complete when:

  - All applications have been handed over

  - AND no critical onboarding work remains

### Cross-Application Awareness

  - Some applications depend on others (e.g. ODA → ODL)

  - Ensure dependencies have been resolved before closing the project

  - If one application caused delays, ensure impact is reflected in:
    
      - project health
    
      - reporting

### Common Mistakes to Avoid

  - Closing a project while an application is still incomplete

  - Setting Project Health without reviewing all applications

  - Ignoring minor issues that become Customer Support problems later

  - Moving project to archive before confirming all handovers

### Notifications Triggered

Internal:

  - Project appears as completed in dashboards

  - Removed from active onboarding tracking

### Final Outcome

  - All applications successfully handed over to Customer Support

  - Project marked as complete

  - Project moved to Completed / Archived space

  - Reporting reflects final onboarding outcome

# SECTION 8 — TEMPLATE VERSION CONTROL

## 8\. Tracking Changes to the Onboarding Template

### Purpose

Every change to the “Project Name” onboarding template is recorded, so
we always know what changed, when, and whether it affects the middleware
— with a rollback path if a change ever causes a problem.

### Where It Lives

The record is a ClickUp Doc, **Template Version Control — Change Log**,
at the space level in the Onboarding Templates space (outside the
Project Name folder, so it is never cloned into client projects).

How to find it:

  - **Onboarding Templates space → Docs → “Template Version Control —
    Change Log.”**

  - Direct link:
    https://quorum.clickup.com/9014937995/docs/8cna2cb-209294

The Doc has three pages:

  - Change Log (history),

  - Current Baseline (system-managed — do not edit),

  - and Runbook (full instructions).

### How It Works

A baseline snapshot of the template lives in the Doc. When the template
changes, the change is diffed against that baseline, logged with a
version bump, the reason, and an “Affects middleware?” flag, and the
baseline is refreshed. Because the baseline lives in ClickUp, everyone
works from the same shared reference.

### Checklist

  - Before editing, duplicate the template folder into the Template
    Archive (version + date) as a rollback point

  - Make the change in the template

  - Ask Cowork to “log the template changes” and add a one-line why see
    prompt in runbook

  - Review the new entry in the Change Log page

  - If flagged Affects middleware: YES, notify the middleware owner
    before it is used

  - If it should apply to future projects, update the reusable template
    (Folder → ⋯ → Templates → Update existing Template)

### Common Mistakes to Avoid

  - Editing the Current Baseline page by hand (only Cowork updates it;
    restore via page history)

  - Renaming/removing lists or tasks without flagging middleware impact
    (breaks Teams routing + middleware)

  - Not logging a change — the reason and context get lost

  - Treating the baseline as a backup — rollback comes from the Template
    Archive and ClickUp’s 30-day Trash
