# SDD Agent Project Template

Template for AI-assisted Specification-Driven Development.

## Structure

- `AGENTS.md` — project-wide instructions for AI agents
- `.sdd/SKILL.md` — SDD operating procedure
- `.sdd/constitution.md` — project principles
- `.sdd/specification.md` — project-level specification
- `.sdd/requirements.md` — requirements and acceptance criteria
- `.sdd/architecture.md` — architecture and interfaces
- `.sdd/tasks.md` — executable work items
- `.sdd/status.md` — current development state
- `.sdd/handoff.md` — continuity between agents
- `.sdd/decisions/` — architecture decision records

## Getting started

1. Customize `constitution.md`.
2. Fill `specification.md`.
3. Define requirements in `requirements.md`.
4. Define architecture in `architecture.md`.
5. Create tasks in `tasks.md`.
6. Have the agent follow `.sdd/SKILL.md`.
7. Keep `status.md` current.
8. Update `handoff.md` before changing agents or stopping work.

## Recommended Git practice

Commit specification and code changes together when they implement the same approved requirement, so the repository preserves the relationship between intent and implementation.
