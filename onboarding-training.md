# Onboarding System — Training Content

**Onboarding System: Training Content**

Salesforce → ClickUp Onboarding Workflow

*Draft, in progress*

1\. System Overview

Onboarding is the process of taking a new customer from a signed deal to
a fully set-up, live client on our systems. The onboarding system
connects Salesforce and ClickUp so that this handover happens
automatically and consistently, with nothing falling through the cracks
between sales and the onboarding team.

The system works in two phases. First, it gives the onboarding team
early visibility of deals in the pipeline: as a Salesforce opportunity
moves into the Commercial Negotiation and Contract Negotiation stages,
it appears in ClickUp's Onboarding Opportunities space, so the team can
see what's coming before a deal is won. Then, once the opportunity is
marked Won in Salesforce, it converts into a full onboarding project in
ClickUp, pre-filled with the customer's details. The onboarding team
works that project through to completion, and when everything is done
the record is closed back off to Salesforce, so both sides always stay
in sync.

**What the system does, at a glance**

  - Tracks Salesforce opportunities in the Onboarding Opportunities
    space as they reach Commercial and Contract Negotiation, giving the
    team forward visibility of what's coming.

  - Converts an opportunity into a full onboarding project once it's
    marked Won in Salesforce.

  - Auto-populates the project with customer and deal details pulled
    straight from Salesforce (including MEDPICC information).

  - Gives the team a structured project, summary tasks, statuses, and a
    Teams channel, to run the onboarding.

  - Notifies the right people when a project is created and as it
    progresses.

  - Closes the record back to Salesforce once all tasks are complete and
    handover notes are added.

  - Provides dashboards and views so account managers, executives, and
    clients can see progress without digging through ClickUp.

**Who uses it**

  - Onboarding / project managers, run the projects day to day.

  - Account managers, track progress on their clients' projects.

  - Executives, see a high-level view across all onboarding.

  - Clients, view progress on their own onboarding, ring-fenced to their
    folder.

**Why it matters**

The system gives us one consistent, repeatable onboarding process. It
reduces manual re-keying and errors, makes progress visible to everyone
who needs it, and ensures every customer gets the same structured
experience from deal close to go-live.

2\. Roles & Responsibilities

Access to the onboarding workspace is managed through three ClickUp
groups. Which group a person belongs to determines what they can see and
do.

**Onboarding Admin**

Holds the admin controls for the workspace. This group configures the
system, manages access and permissions, maintains dashboards and views,
and looks after the settings that keep the Salesforce-to-ClickUp
integration running. Admins are responsible for the setup that everyone
else relies on.

**Onboarding**

The onboarding / project managers who run projects day to day. They pick
up a project once it converts from a won opportunity, work the tasks
through to completion, keep statuses and health up to date, add handover
notes, and close the record back to Salesforce when the customer is
live.

**Account Managers**

Track progress on their clients' onboarding without managing the tasks
themselves. They work primarily from the dashboards and views, seeing
where each project is, what's completed, what's outstanding, and the
expected completion date, and raise questions with the project manager
when needed.

3\. The End-to-End Flow

This is the full journey a customer takes, from a deal in the Salesforce
pipeline to a live client handed back to Salesforce. The diagram below
summarises it; the steps underneath walk through each stage.

1.  **Opportunity created (Salesforce).** A salesperson raises the
    opportunity and works it through the early pipeline stages.

2.  **In Negotiation (Salesforce → ClickUp).** Once the opportunity
    reaches Commercial or Contract Negotiation, it syncs into the
    ClickUp Opportunities list, giving the onboarding team forward
    visibility of what's coming before the deal is won.

3.  **Marked Won (Salesforce).** When the stage flips to Won, the
    opportunity is ready to become a live onboarding project.

4.  **Onboarding project created (ClickUp).** The system creates the
    project automatically, with the intake details auto-populated from
    Salesforce so the team starts with the customer's information
    already in place.

5.  **All tasks completed (ClickUp).** The onboarding team works the
    project through, tasks, statuses and health, until the customer is
    set up.

6.  **Handover notes check.** The record can only close once handover
    notes are added. If they're missing, it stays open until the notes
    are in place.

7.  **Closed back to Salesforce.** With tasks complete and handover
    notes added, the record is closed off and returned to Salesforce,
    keeping both systems in sync.

*End-to-end onboarding flow: Salesforce to ClickUp and back.*

4\. Opportunity Tracking (Pre-Win Visibility)

The onboarding team doesn't wait until a deal is won to know about it.
While an opportunity is still being negotiated in Salesforce, it already
shows up in ClickUp, giving the team a forward view of what's in the
pipeline so they can plan and resource ahead of time.

**How it works in Salesforce**

Every opportunity in Salesforce has a Stage field. As the salesperson
moves the deal along and selects Commercial Negotiation or Contract
Negotiation, the opportunity syncs across into the ClickUp Opportunities
list (in the Onboarding Opportunities space). No extra action is needed,
changing the stage is what drives it.

*Salesforce, selecting the opportunity Stage. Commercial and Contract
Negotiation are the stages that surface the deal in ClickUp.*

**What you see in ClickUp**

In the Onboarding Opportunities space, the Opportunities board is
grouped into status columns that mirror the Salesforce stages exactly,
To Do, Commercial Negotiation, Contract Negotiation and Won. Each card
is an opportunity, carrying its MEDPICC detail so the team can see the
shape of the deal at a glance. As the stage changes in Salesforce, the
card moves across the board.

*ClickUp, the Opportunities board, with columns mirroring the Salesforce
stages.*

**Why it matters**

This forward visibility lets the onboarding team prepare before a deal
closes rather than starting cold once it's won. When the stage finally
flips to Won, the opportunity converts into a full onboarding project,
the point where the end-to-end flow in Section 3 picks up.

5\. Intake & Forms

Before an opportunity is set to Won, the user completes the App
Onboarding Form in Salesforce. This is where the details that drive the
ClickUp project are captured, so completing it accurately and fully is
what makes the auto-populated onboarding project correct.

**Selecting the applications**

At the top of the form, Application Name lets the user tick which
applications the client is onboarding, AP Workflow, Data Hub, Data Hub
Premium, Dynamic Docs, Execute, OGsql Conversion, On Demand Accounting,
On Demand Land and On Demand Well Operations. Each application ticked
here adds its own section to the form below.

*The App Onboarding Form in Salesforce, tick the applications, then
complete a section for each.*

**Per-application details**

For each selected application, the form captures the App Client Contact
Name and App Client Contact Email (both required), Milestone Details,
Additional Note Details, and whether a partner is involved (App Is
Partner Involved). These map across to the matching application in the
ClickUp project.

**General information**

The General Information section captures Applications Existing (move the
client's existing applications from Available to Chosen), the Copy of
Contract (required), and General Notes.

*General Information, existing applications, the required Copy of
Contract, and general notes.*

**Submitting**

Submitting the form saves these details against the opportunity. When
the opportunity is later marked Won, this is the data that flows into
ClickUp to create and pre-fill the onboarding project, so anything
missing or wrong here shows up in the project.

6\. ClickUp Project Structure

Every onboarding project follows the same structure in ClickUp, so
anyone on the team can open a project and immediately know where to find
things.

**Space and folders, one folder per client**

All live projects sit in the Onboarding Projects space. Each client has
its own folder, named with the company and its account number, for
example, Aethon Energy Operating LLC \[A-022888\]. A folder is a
self-contained project: everything for that client lives inside it.

*The Onboarding Projects space, one folder per active client, named with
company and account number.*

**Lists, one per application**

Inside a folder, work is split into lists. The first is always Project
Summary, and the rest are one per Quorum application the client is
onboarding, for example OGSql → ODA, DynamicDocs, Execute AFE, On Demand
Accounting, On Demand Land, On Demand Production, On Demand Well and
zdSCADA. The number of lists varies by client, depending on which
applications they have bought. The tasks in each list are the
configuration, testing and go-live steps for that application, and key
stages are flagged as milestones, Sales to CS Handoff, Kick-Off, the
numbered Steps and Go-Live.

*A project folder (ACME Oil Pty Ltd) with its Project Summary list and
one list per active application.*

**Project summary**

The Project Summary list (the first list in every folder) holds a
summary task for each application the client is onboarding, each tagged
with its application. Together these give the project's overall health,
the expected end date and a short summary of where things stand, the
information that surfaces at the top of the AM Overview and the
dashboards, so it is worth keeping current.

*The Project Summary list, one summary task per application, each tagged
with its application.*

**What's on a summary task**

Each summary task carries a set of custom fields that capture everything
about that application's onboarding, the client and contacts, the
salesperson, project health, tier and churn risk, expected vs actual
start and end dates, blockers, integration setup and mapping status, app
partner details, and the handover fields (H\_Ready for Handover,
H\_Handover Captured and H\_Notes). The MEDDPICC detail and the handover
notes come in as attachments on these fields, so the full context of the
deal lives right here on the task. This is where the onboarding team
keeps each application's status up to date.

*Custom fields on an application summary task (OGSql → ODA Summary),
including MEDDPICC and the H\_ handover fields.*

7\. Setting Up & Starting the Application

Before execution begins, the project manager sets the application up so
onboarding starts with clear ownership, a timeline and full context.
This work happens on the Application Summary task, validating and
completing the data that came across from Salesforce. This step is about
understanding what was sold, not starting the work yet.

**Setup checklist**

  - Review the Salesforce data on the Application Summary task and
    confirm the application is relevant (not mistakenly included).

  - Assign yourself as the Application Owner, and add supporting
    onboarders if required.

  - Confirm the Client Contact Name and Email, Applications Sold and
    Existing, Contract Closed Date and Copy of Contract.

  - Review Application Notes, Milestone Details, and the Integration
    Setup / Mapping & Matching requirements.

  - Check whether a Partner is involved and confirm the Partner Type and
    Name.

  - Review the Expected Start and Expected End planning dates, leave
    Actual Start and End, which are set automatically.

  - Set the initial Application Health to Green (On Track).

  - Create the Teams channel for the project and paste its link into
    team\_notify\_id.

*The notification fields, set team\_notify\_id to the Teams channel
link. The Notify on Start/End messages shown here are preset in the task
templates.*

**Setting up the Teams notifications**

Each application's Start and End notifications post to the Teams channel
set on the Application Summary task. The messages themselves are preset
in the task templates, so you don't write them per project, the one
thing you must do at startup is point the project at the right channel:

1.  In Teams, create or choose the channel and name it (for example
    "Onboarding - \<Client\>").

2.  Next to the channel name, click the ... menu and choose Copy link.

3.  Paste the link into the team\_notify\_id field on the Application
    Summary task.

The Notify on Start and Notify on End toggles and their messages sit on
the individual tasks in the application lists and are already set in the
template, there is no per-project message to write.

**Starting onboarding**

The official start trigger is setting the Application Summary task to In
Progress, this activates the timeline, tracking and dashboards. Set the
Due Date based on the length of the onboarding, and don't change it once
set. Then set the Start Date on the first execution task and move it to
In Progress; this populates the Actual Start and activates ClickUp's
downstream scheduling across the dependency chain.

**Watch out for**

The Salesforce data may be incomplete or slightly incorrect, you are
responsible for validating and correcting it early, and for flagging
anything that looks wrong before proceeding. The most common setup
mistakes are leaving Application Health unset, not assigning ownership
clearly, ignoring partner involvement, and starting work before
reviewing the contract and milestones.

8\. Working the Project

Once a project is live, the onboarding team works through the tasks in
each application list. The tasks are pre-built from the template, so the
team follows a consistent path for every client rather than building the
plan from scratch.

**Tasks are organised into phases**

Each application list is broken into phases that run in sequence, Phase
1 (handoff, kick-off and environment setup), Phase 2 (admin training and
master-file configuration), and Phase 3 (processing, training and
pre-transition). Tasks follow a consistent naming pattern, such as ODA
\> Step 1 - Admin Training, so anyone can see where a task sits in the
flow.

**Milestones and checkpoints**

Key tasks are flagged as milestones (for example the Project Kick-Off
and the Master File step), and OPP checkpoint tasks mark the review
points along the way, Master File Complete, Mid-Point Review and
Pre-Transition Review. These are the moments to confirm the project is
on track before moving on.

**Tracking each task**

Every task carries a status, an assignee, start and due dates, a
duration and a time estimate, so both progress and effort are visible.
The team updates statuses as they work, and each phase rolls up a total
time estimate. The same list can be viewed as a Board, Gantt or Timeline
for scheduling, alongside the Operations and Client Dash views, but the
day-to-day work happens here in the list.

*Example, the On Demand Accounting task list, organised into phases with
milestones, checkpoints, durations and time estimates.*

9\. The Handover Process

Handover is how a completed application is transferred to Customer
Support with the full context of what happened during onboarding. The
key principle is that it is captured continuously throughout onboarding,
not written at the end.

**Capturing the handover (H\_Notes)**

Throughout onboarding, keep the standard handover template up to date.
Capture the overall onboarding and UAT status, any unique configuration
notes and integrations enabled, risks and unresolved issues, client
sentiment and champions, at-risk indicators and follow-up
recommendations, and the ClickUp project link. When something important
happens, ask whether Customer Support will need to know it later, if so,
record it. Save the completed template and attach it to the H\_Notes
field on the Application Summary task, always replacing any older copy
so the latest version is the one attached.

**Completing and triggering the handover**

When the application is ready, confirm all relevant tasks are complete
or documented, confirm the Actual End is captured, confirm the latest
handover template is attached to H\_Notes, do a final review of the
Application Summary task, and then check H\_Ready for Handover.

**What happens when you check Ready for Handover**

  - A webhook fires and the middleware collects the H\_Notes attachment
    and the handover flags.

  - The data is pushed into Salesforce.

  - On success, H\_Handover Captured is set to true and the record
    reflects the completed handover.

  - If H\_Notes is missing, the handover fails: the automation posts a
    handover-failed alert and unchecks the box, so the record cannot
    return to Salesforce until notes are attached.

**Important**

The application does not need to be 100% complete, but it must be clear,
documented and ready for Customer Support to take ownership. Don't check
H\_Ready for Handover if key information is missing, configuration
details are incomplete, or major risks are undocumented, you only get
one clean handover.

*The handover fields on the Application Summary task, H\_Ready for
Handover, H\_Handover Captured and the H\_Notes attachment.*

10\. Dashboards & Views

Dashboards give each audience a read-only view of progress without
having to navigate ClickUp. Each is shared as a link that can be
bookmarked.

**Account Manager dashboard**

The AM dashboard shows the status of all onboarding projects at a
glance, project, health and expected end date, with what is completed
and what is still outstanding. Account managers open it from a single
link; they don't manage the tasks themselves. Drilling into a project
opens its AM Overview, scoped to that folder.

**Executive dashboard**

The exec dashboard gives leadership a high-level view across all
onboarding. Like the AM dashboard, it is shared as a link, the recipient
lands directly on the dashboard rather than in the space.

**Client views**

A client can be given a view of their own project, ring-fenced to their
folder so they only see their own onboarding (covered under Access &
Permissions). This is typically shared as a specific view or dashboard
rather than access to the whole space.

**Sharing a view**

To share a view, right-click it and choose Copy link to view; the
recipient can bookmark it. Keep the project summary at the top of any
task-list widget so it is the default a viewer sees, and note that
per-product widgets can be filtered by application (for example ODA vs
ODL).

*AM Dash, the portfolio of onboarding projects, each with a progress
bar.*

*AM Overview, a single project: completed tasks, what's left to do, and
the project summary with health and expected end.*

11\. Access & Permissions

Access to ClickUp is controlled so that each audience sees only what
they should. There are a few moving parts, Okta, guest vs member access,
and ClickUp seats.

**Okta login**

IT currently requires Okta for access to the ClickUp workspace, so
clients and external users log in through Okta. Onboarding initiates the
client's Okta login when the database is set up, before inviting them to
the ClickUp project.

**Guests vs members, and seats**

  - Guest, view-only, can see what is shared with them and does not
    consume a ClickUp seat. This is how clients and non-user executives
    are given visibility.

  - Guest, edit, can make changes to what is shared; confirm current
    seat treatment before using at scale.

  - Member / limited member, internal users; consumes a seat.

**Client ring-fencing**

A client is only ever given access to their own folder. Because they see
only what is shared with them, they can't see other clients' projects in
the same space, their access is ring-fenced to their folder.

Note: the Okta requirement on guest access is being reviewed with IT so
that non-user executives and clients can be added more easily. Until
that is lifted, guests still need Okta access to open a shared view.

**Sharing a folder with a client (view-only guest)**

To give someone access to a folder, open the folder's ... menu and
choose Sharing & Permissions.

*The folder ... menu, choose Sharing & Permissions.*

In the Share this Folder dialog, enter the person's email, set Invite as
to Guest, and choose View only, then Send Invite.

*Share this Folder, invite by email, or copy the private link.*

*Invite as Guest, View only, view-only guests are free and don't count
towards seat limits.*

12\. Notifications & Teams

The Onboarding space runs a set of automations that watch for task and
field changes and call a webhook, which posts a message into the
project's Microsoft Teams channel. This keeps the wider team informed
without anyone having to sit in ClickUp. The automations fall into three
groups.

**Task-level notifications**

  - **Task Started,** a task moves off Not Started and its Notify on
    Start field is checked.

  - **Task Completed,** a task moves to Complete and its Notify on End
    field is checked.

  - **Task Blocked,** a task's status changes to Blocked.

  - **Task Unblocked,** a task moves back out of Blocked.

**Application-level notifications (on the summary task)**

  - **New Application Onboarding Started,** the summary task moves from
    Not Started to In Progress.

  - **Application Onboarding Completed,** the summary task moves from In
    Progress to Complete.

  - **Application Blocked / Unblocked,** the Blockers field is set or
    cleared.

  - **Application Health,** the Project Health field changes.

**Handover automations**

  - **Handover readiness guard,** if H\_Ready for Handover is checked
    but H\_Notes is not set, the automation posts a handover-failed
    alert and unchecks the box, blocking the handover until notes are
    added.

  - **Handover trigger,** if H\_Ready for Handover is checked and
    H\_Notes is set, it fires the handover webhook (returning the record
    to Salesforce) and resets the box.

**How they work**

Each automation follows the same shape, a trigger (a status or
custom-field change), an optional condition, and an action that calls a
dedicated "Onboarding Teams Notification" webhook. The Notify on Start /
Notify on End toggles and the message templates live on the summary
task's fields, and team\_notify\_id sets the Teams channel the messages
post to. Turning a toggle off suppresses that message for the project.

*Example automation, Notify on Task Started: when a task leaves Not
Started and Notify on Start is checked, it calls the Task Started Teams
webhook.*

13\. Edge Cases

A few less-common situations to be aware of:

  - **Multiple applications.** A project can have several application
    lists and summary tasks; each is worked and handed over on its own.

  - **Partners involved.** Confirm the Partner Type and Partner Name
    early; unflagged partner involvement causes delays later.

  - **Cross-application dependencies.** Some applications depend on
    others (for example ODL depends on ODA). Don't start dependent work
    until the prerequisite tasks are complete, and don't remove
    dependency relationships, they drive the Gantt and timeline.

  - **Large attachments.** Content loaded into attachment fields has a
    character limit; be aware of where long content is cut off.

  - **No duplicates.** When resubmitting a record back to Customer
    Support / Salesforce, make sure it is not duplicated.

14\. Troubleshooting / FAQ

Common snags and how to resolve them. This section will grow as UAT and
live use surface new issues.

  - **A Teams notification did not fire.** Check that the task and its
    Project Summary share a tag, that a "project summary" list exists in
    the folder, and that the Team Notify field holds a valid Teams link
    (with groupId= and /channel/{id}/). See Appendix A of the playbook.

  - **Expected End is not syncing.** Confirm the triggering task has a
    Due Date and the summary field is named exactly "Expected End."

  - **A health or blocker card is blank.** Set the Project Health and/or
    Blockers fields on the task; otherwise the card shows "No
    health/blocker set."

  - **The team was not notified of a brand-new project.** ClickUp has no
    native "folder created" automation trigger; this notification is
    best handled by the middleware that creates the folder (planned
    enhancement).

  - **Handover will not go through.** The record cannot return to
    Salesforce until the completed handover template is attached to
    H\_Notes.

15\. Archiving & Completion

Project-level completion is the onboarding manager's responsibility,
once every application has been handed over.

**Closing a project**

  - Review every Application Summary task and confirm each has been
    handed over (H\_Handover Captured = true).

  - Review Application Health across all applications and set the
    overall Project Health.

  - Confirm no critical blockers remain and that all required handovers
    to Customer Support are complete.

  - Do a final review of the Project Summary fields and confirm the
    project is ready for closure.

  - Move the project to the Onboarding Complete space in ClickUp.

**Completion criteria**

A project is complete when all applications have been handed over and no
critical onboarding work remains. Resolve any cross-application
dependencies before closing, and make sure any delays are reflected in
project health and reporting. Once moved to Onboarding Complete, the
project drops out of active tracking and the dashboards reflect its
completion.

16\. Glossary / Key Terms

  - **MEDDPICC / MEDPICC,** the sales qualification detail (Metrics,
    Economic buyer, Decision criteria, Decision process, Paper process,
    Identify pain, Champion, Competition), carried across from
    Salesforce as an attachment on the summary task.

  - **ODA / ODL / ODP / ODW,** On Demand Accounting, Land, Production
    and Well, the Quorum applications a client onboards. Others include
    Execute / AFE, DynamicDocs, zdSCADA and OGSql.

  - **Application Summary task,** the per-application record holding
    health, dates, notification fields and handover fields.

  - **Project Summary list,** the first list in a project folder,
    holding one summary task per application.

  - **H\_Notes,** the handover notes template, attached to the summary
    task and collected at handover.

  - **H\_Ready for Handover / H\_Handover Captured,** the checkbox that
    triggers handover, and the flag set to true once the middleware
    pushes the record to Salesforce.

  - **team\_notify\_id (Team Notify),** the field holding the Teams
    channel deep link that notifications post to.

  - **Middleware,** the integration that moves data between Salesforce
    and ClickUp and back.

  - **Handover,** the transfer of a completed application to Customer
    Support.

  - **Idle,** an application with no meaningful activity or stalled by
    client or partner delays.
