# Reusable prompt — M4AW weekly call agenda

Paste this at the start of a session on the Thursday of the call.

---

Build the agenda for today's Made For A Woman × KR8 weekly call.

**1. Establish the baseline.**
- Read the most recent agenda in `agendas/` and the most recent recap in `recaps/`
  in this repo — that is the format and the starting task list.
- Find last week's agenda doc in Google Drive (`title contains 'Weekly Meeting
  Agenda'`) and read it. The master log doc is large — extract it with jq/python
  rather than reading it whole.
- Read the calendar event to confirm date, time, attendees and any change to the
  standing agenda in the description.

**2. Pull updates from every workspace, for the period since the last call.**
- Gmail: the client thread(s), and the auto-generated meeting notes for last
  week's call. Read the client's own messages in full — do not work from snippets.
- Slack: `#m4aw-x-kr8` (client-facing), `#m4aw-internal`, `#m4aw-x-ads`,
  `#m4aw-x-developers`, `#new-dev-x-m4aw-web`, plus `#internal-kr8` for blockers.
- Notion: the Made For A Woman client hub task board — query open items with
  status, owner, due date and notes.

**3. Audit before writing. This is the part that matters.**
- For every date, price, threshold and decision, find the *most recent*
  authoritative source. The client's own word on their own launch dates, budgets
  and priorities overrides our internal tracking, even when our note is newer.
- Explicitly check whether last week's decisions have since been reversed by the
  client. Do not re-present a settled decision as "decision needed".
- Check whether anything we promised in writing has actually been delivered.
  Overdue items owed to the client go in the agenda as overdue, named honestly.
- Verify any document before quoting it — templates and sample data circulate
  internally and must never reach a client agenda.
- Confirm whether the client's last substantive message has been answered.

**4. Write it to match the template exactly, for copy-paste.**
- Output plain text to `agendas/YYYY-MM-DD-agenda-plain-text.txt`, blocks labelled
  TITLE CELL / DATE / ATTENDEES, then numbered sections separated by `====` rules.
- No markdown bold or asterisks — the Google Doc applies its own formatting.
- Em dashes (—), not hyphens, in headings and mid-sentence. `×` in the title.
- One line per bullet, starting `- `. Every line short enough to read aloud.
- Section titles carry the decision: "— Decision Needed", "— Confirmed", "— Parked".
- Open the agenda with the performance snapshot, and close with
  "Next Steps — Owners & Dates".

**5. Report separately.** Write the audit trail to
`agendas/YYYY-MM-DD-audit-notes.md`: what you corrected and why, what you
deliberately excluded, and anything I need to resolve before the call. Commit and
push both files. Do not post anything to Slack, Notion or email without asking.
