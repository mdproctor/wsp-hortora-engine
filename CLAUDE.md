# garden-engine Workspace

**Name:** garden-engine
**Project repo:** /Users/mdproctor/claude/hortora/garden-engine
**Workspace type:** public

## Session Start

Run `add-dir /Users/mdproctor/claude/hortora/garden-engine` and `add-dir /Users/mdproctor/claude/public/hortora/garden-engine` before any other work.

## Artifact Locations

| Skill | Writes to |
|-------|-----------|
| brainstorming (specs) | `specs/` |
| writing-plans (plans) | `plans/` |
| handover | `HANDOFF.md` |
| idea-log | `IDEAS.md` |
| java-update-design / update-primary-doc | `design/JOURNAL.md` (created by `work-start`) |
| adr | `adr/` |
| write-content | `blog/` |

## Structure

- `HANDOFF.md` — session handover (single file, overwritten each session)
- `IDEAS.md` — idea log (single file)
- `specs/` — brainstorming / design specs (superpowers output)
- `plans/` — implementation plans (superpowers output)
- `snapshots/` — design snapshots with INDEX.md
- `adr/` — architecture decision records with INDEX.md
- `blog/` — project diary entries with INDEX.md
- `design/` — work-start creates JOURNAL.md and .meta here per branch

## Git Discipline

Two git repositories are active in every session:
- **Workspace** (`/Users/mdproctor/claude/public/hortora/garden-engine`) — plans, blog, snapshots, handover
- **Project repo** (`/Users/mdproctor/claude/hortora/garden-engine`) — source code, ADRs, specs

Never rely on CWD for git operations. Always use explicit paths:
```bash
git -C /Users/mdproctor/claude/public/hortora/garden-engine add <file>   # workspace
git -C /Users/mdproctor/claude/hortora/garden-engine add <file>          # project
```

## Rules

- All methodology artifacts go here, not in the project repo
- Workspace branches mirror project branches — switch both together

## Routing

| Artifact   | Destination |
|------------|-------------|
| adr        | project     |
| specs      | project     |
| blog       | workspace   |
| plans      | workspace   |
| design     | workspace   |
| snapshots  | workspace   |
| handover   | workspace   |

@/Users/mdproctor/claude/hortora/garden-engine/CLAUDE.md
