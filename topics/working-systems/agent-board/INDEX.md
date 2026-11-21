---
type: sop
status: template
---

# Agent Board

Optional queue for repeatable work that an agent can prepare and a human can review. Create a board in your task system only when the workflow below solves a real coordination problem.

## Suggested stages

| Stage | Meaning |
|---|---|
| Intake | Request captured, scope unverified. |
| Needs information | Waiting for essential context or owner decision. |
| Ready | Instructions and sources support a bounded preparation step. |
| In progress | Exactly one worker owns preparation. |
| Human review | Proposed result and evidence ready for approval. |
| Done | Verified outcome recorded; further changes require a new instruction. |

Suggested fields: owner, priority, due date, execution lane, status, source link and definition of done. Start with manual review of one ticket. Separate *preparing* a change from *executing* a change in an external system.

## Ticket path

1. Verify the request and search for duplicates.
2. Confirm the task's board and exact stage before claiming it. An automated dispatcher needs an exclusive lock, capacity limit, occurrence ledger and a retry-safe reservation.
3. Give the specialist a dedicated visible work surface and brief: outcome, sources, permissions and definition of done.
4. Save the proposal, evidence, blockers and next action in a linked case. Ask for review before any action beyond granted permissions.
5. Verify the result in its source system, then update the board and record reusable feedback.

Scheduled checks need explicit timezone, windows, missed-run reporting and read-back. Do not infer a scan from a quiet chat. The board here has **no configured external ID, automation or write permission**.
