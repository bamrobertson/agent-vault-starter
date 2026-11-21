# Agent Vault Starter

An empty, Obsidian-friendly framework for working with an AI Chief of Staff and specialist agents. It contains structure and instructions, not anyone's tasks, messages, company procedures, credentials or connected accounts.

## Start here

1. Clone this repository and open the folder as an Obsidian vault (optional; Markdown works without Obsidian).
2. Read [AGENTS.md](AGENTS.md) and [INDEX.md](INDEX.md). Replace the generic working-scope descriptions with your own. Keep private and work information in their respective sections.
3. Add one project under `topics/projects/` and link it from that folder's index. Put current facts and source links in its note; put a dated decision in `decisions/` when a rule actually changes.
4. Set up [Chief of Staff](topics/working-systems/Chief%20of%20Staff.md) as a **manual, read-only** chat first. Give it only the sources it needs and check its plan against reality. Add a schedule only when the environment, timezone, destination and source access have been tested.
5. If you have repeatable tasks, use [Agent Board](topics/working-systems/agent-board/INDEX.md). Start with manual review of one ticket and an explicit approval boundary. Automate pickup only after you can verify state, deduplicate retries and detect missed runs.
6. Record integrations in [Integrations](topics/working-systems/integrations/INDEX.md). Never paste keys into notes or Git. A connection being readable does not mean it can write or that an automated run can access it.

## Folder map

| Path | Purpose |
|---|---|
| `AGENTS.md`, `INDEX.md` | Short agent rules and navigation. |
| `topics/projects/`, `topics/knowledge/` | Current work and source-backed knowledge. |
| `topics/working-systems/` | COS, Agent Board and integration guidance. |
| `decisions/`, `summary_log.md` | Dated rule changes and meaningful work results. |
| `personal/` | Optional separate personal scope and logs. |
| `_templates/` | Blank notes for projects, decisions, tickets and lessons. |
| `.agents/skills/` | A place for explicitly designed reusable skills; none are installed here. |

Indexes contain prompts to fill in, not sample business data. The empty topic folders are kept by their `INDEX.md` files. `tmp/` is ignored and can be created for disposable task work.

## How the parts work together

The COS helps choose priorities and follow through. A specialist owns one narrow job and returns a source-linked outcome. The board tracks work and human review. Durable decisions and tested lessons update the relevant instructions; an agent should not silently rewrite its own permissions. For independently scheduled specialists, COS reads a compact status record and highlights missing or stale evidence. See [Status contract](topics/working-systems/Specialist%20Status%20Contract.md).

## GitHub and privacy

This repository is a **starter**, never a mirror of your working vault. Create your own private copy before adding real content. If you later make that copy public, review its **entire history**, not only current files; deleting a secret from the latest commit does not remove it from history. Keep runtime state, exports, private messages and credentials out of Git. Review `git status`, staged diffs, filenames and remote visibility before pushing.

No schedules, API permissions, integrations or agents are activated by cloning this repository.
