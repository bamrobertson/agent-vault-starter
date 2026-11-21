---
type: sop
status: template
---

# Specialist status contract

Use a small status summary when a separately scheduled worker reports to COS. It supplements the worker's own ledger and case; it does not replace them.

| Field | Required meaning |
|---|---|
| Checked at | Actual verified run time and timezone. |
| Outcome | Completed, no eligible work, deferred, failed, or pending review. |
| Needs owner | One actionable decision and link, if any. |
| Blocker | Permission, source, timing or uncertain-write issue. |
| Source links | Stable pointers to the work and evidence, with private details kept private. |
| Coverage | Exact sources and scheduled occurrences checked; distinguish missed runs. |

The COS should say “no run recorded” or “partial coverage” when that is the evidence. A quiet specialist chat alone is not proof that a scan ran.
