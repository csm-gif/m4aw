# M4AW weekly call agenda — process prompt (v2)

Paste the block below into a fresh session on the Thursday of the call. It
supersedes v1, which opened with the wrong section, set no length discipline, and
had no client-appropriateness filter. See git history for the original.

---

## Standing facts

Do not re-derive these each week; verify only if something looks off.

- **Call:** Made For A Woman × KR8, Thursdays, 4:30pm CET / 7:30am PST.
  Calendar event "Made For A Woman - Weekly Discussion". Check the event
  description each week — standing agenda changes get recorded there (the paid ads
  review was folded into this call on 9 Sept 2026).
- **Attendees:** Gaia, Olga, Eileen, Madison / Allan, Chima, Maya, Amandeep, Alex.
- **Master agenda log (the template):**
  `docs.google.com/document/d/1xetR07xTjxCTiRwl5gv_G5pXTJJlTdRi6J2whxef6cs`
  Newest week sits at the top. ~50k characters — extract with jq or python, never
  read it whole.
- **Slack:** `#m4aw-x-kr8` (client-facing, the source of truth for client
  decisions) · `#m4aw-internal` · `#m4aw-x-ads` · `#m4aw-x-developers` ·
  `#new-dev-x-m4aw-web` · `#internal-kr8` (blockers).
- **Notion:** client hub `3adbb8409bda80d0a49cf2496b4fee33`; tasks data source
  `collection://8acbb840-9bda-82b9-bf80-8749db2d9462` (filter on the Client
  relation, exclude Done / Live / Cancelled).
- **Repo:** `agendas/` and `recaps/` hold the format and the running task list.

---

## The prompt

Build the agenda for today's Made For A Woman × KR8 weekly call.

### 1. Baseline

Read the most recent agenda in `agendas/`, the most recent recap in `recaps/`, and
last week's agenda doc in Drive. Read the calendar event for date, time, attendees
and any change to the standing agenda.

### 2. Gather everything since the last call

- **Gmail** — the client threads, and the auto-generated notes from last week's
  call. Read the client's own messages in full; never work from snippets.
- **Slack** — every channel listed above.
- **Notion** — open tasks with status, owner, due date and notes.

### 3. Audit. This is the part that earns the agenda.

- **The client outranks our tracking.** On their own launch dates, budgets,
  thresholds and priorities, their latest word wins — even when our internal note
  is more recent. (Sept 2026: Gaia set Drop 2 to the 29th in the morning; an
  internal message still said the 24th that afternoon. She was right.)
- **Check for reversals.** A decision made on last week's call may have been
  undone by email since. Never re-present a settled or withdrawn decision as
  "decision needed".
- **Check what we owe.** Anything promised in writing and not delivered goes in
  as open, with the delivery date.
- **Verify every document before quoting it.** Internal templates circulate
  carrying invented sample figures. If a doc's numbers or conclusions contradict
  the client's own read, it is not their data — exclude it. Never let a sample
  number reach a client agenda.
- **Has their last substantive message been answered?** If not, say so in your
  report — the call is the answer, and that shapes the whole agenda.
- **Never present stale figures as current.** If no fresh numbers exist, label
  them as the last confirmed read and ask for the update live.

### 4. Choose the sections

- **01 is always "Last Week's Actions — Status."** Non-negotiable: opening with
  last week's actions and their status is a standing agreement with the client
  from the 3 Sept 2026 call. Sub-blocks: `Closed`, `Open — KR8`, `Open — MADE`.
- **Close with "Next Steps — Owners & Dates."**
- Between those, use **as few sections as capture the week** — typically three.
  There is no target count. Number them sequentially 01, 02, 03… with no gaps.
- **Each item appears once.** Do not create a separate "with you for review"
  section; those items are `Open — MADE` in 01. If two sections would carry the
  same fact, cut one or point back to the other.
- Section titles carry the state: `— Confirmed`, `— Decision Needed`, `— Parked`.

### 5. Write for the client, not for us

The agenda is client-facing. Include only what they need to decide, act on, or be
reassured by. Cut:

- **Internal operational mechanics** — how we'll restructure ad sets, which
  developer takes which ticket.
- **Granular build state** — "email 1 live, 2–5 pending design approval" becomes
  one line about what is waiting on them.
- **Why we were late.** Overdue items give the delivery date only: "Press page
  layout — will be submitted to you today." Not the slippage history.
- **Their own settled decisions**, beyond a one-line acknowledgement.
- **Closed items with no consequence for them**, and internal context such as who
  is travelling.

Budget: aim for ~30 lines total. Six or seven bullets per section, ~13 for 01.
If a line would not change what someone does or thinks, delete it.

### 6. Format for copy-paste

Write plain text to `agendas/YYYY-MM-DD-agenda-plain-text.txt`:

- Header, then blocks labelled `TITLE CELL`, `DATE`, `ATTENDEES`, then numbered
  sections separated by `============` rules.
- **No markdown bold or asterisks** — the Google Doc applies its own formatting.
- Em dashes (—) in headings and mid-sentence. `×` in the title line.
- One line per bullet, starting `- `, short enough to read aloud.
- **An owner in parentheses after every open action item**, both sides:
  `- Product video format spec — to be done today. (Maya)`

### 7. Consistency check before you save

- Does any two-section pair state the same thing? Cut one.
- Does every commitment use the same wording everywhere it appears? If a date
  moves from "on this call" to "after this call", propagate it to Next Steps so
  the agenda cannot contradict itself.
- Is every number, date and name traceable to a source you actually read?

### 8. Deliver

Write the audit trail to `agendas/YYYY-MM-DD-audit-notes.md`: what you corrected
and why with sources, what you excluded and why, and what I must resolve before
the call — especially **client priorities blocked internally**, which belong in my
report and never in the client agenda.

Commit and push both files. Do not post to Slack, Notion or email without asking.
