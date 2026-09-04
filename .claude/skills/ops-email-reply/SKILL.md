---
name: ops-email-reply
description: Draft Chima's client email replies in KR8 operations style — status first, 2-3 bullets, no waffle, no apologies, no new work for the team. Use whenever replying to or acknowledging a client email (meeting recaps, action-item lists, status chases, access or delivery questions), or when asked for "a quick acknowledgement", "reply to this email", or "draft a response" to a client thread.
---

# Operations Email Reply (Chima / KR8)

Every reply must read like operations management: the client learns what is done, what is
pending with an owner and date, and the single thing they need to do.

## Before writing

Verify status from the systems of record, never from memory:
1. **Slack** — the client channel and the internal channel for what was posted, confirmed or resolved.
2. **Notion** — that the tasks referenced exist with owner and deadline.
3. The thread itself — every point the client raised.

Never write "done" for anything not confirmed in one of those. If a point is still open, say
it is open with the date it lands.

## Structure

```
Hi [Name],

[One line: what is DONE. No thanks-preamble before it.]

• [Point 1 — decision or status, with owner/date if pending]
• [Point 2]
• [Point 3 max]

[One line: the single question or confirmation needed from them.]

Best regards,
Chima
```

## Rules

- **Status first.** The first line after the greeting states what is complete. Not "thank you
  for your time", not "as discussed", not "I wanted to follow up".
- **2–3 bullets, maximum.** Each bullet is one decision or one status. Merge related items
  rather than adding a fourth bullet. Anything longer belongs in Notion, linked.
- **No waffling, no internal process.** Cut "we are working on", "we will look into", "our
  team is currently", "just to circle back". Who and when, or nothing. Never explain KR8's
  internal routing, staffing, tooling or why something slipped.
- **No apologies.** No "sorry for the delay", "apologies for the confusion", no self-blame,
  no over-thanking. Acknowledge and state the fix date instead.
- **Never create work for the team by email.** Do not commit KR8 people to new scope, new
  deadlines, or new deliverables that are not already in Notion with an owner. If the client
  asks for something new, the reply says it goes into Notion for scoping — it does not
  promise a date.
- **One ask, at the end.** Close with exactly one thing the client must confirm or decide.
  If nothing is needed from them, say "Nothing needed from you" and stop.
- **Owners and dates, always.** Any pending item named in the email carries an owner and a
  date, matching Notion exactly.
- **Plain, factual tone.** Short sentences. No exclamation marks, no hedging adverbs
  (hopefully, ideally, potentially), no filler closers ("looking forward to building on the
  great work together").

## Handling common cases

- **Client asks "is X fixed?"** — Answer yes or no in the first line. If partly, name what
  works and what does not, and the date for the rest.
- **Client sends a task list** — Confirm it is reflected in Notion with owners and deadlines.
  Do not restate the list in the email.
- **Client raises a problem** — State the current status, the owner, the date. No cause
  analysis, no apology.
- **Client duplicates something already handled in Slack** — Say it was confirmed in Slack on
  [day] so both records match. One line.
- **Something is blocked on the client** — Put it in the closing ask, not in a bullet.

## Delivery

Create a Gmail **draft** on the existing thread — never send without explicit approval. Keep
the original cc list unless told otherwise. Report to Chima which claims were verified and
where.

See `reference/example.md` for a worked example.
