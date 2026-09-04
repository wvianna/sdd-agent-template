# AGENTS.md — Project Agent Instructions

## Mandatory SDD workflow

This project uses Specification-Driven Development (SDD).

Before making significant changes, the agent MUST read:
1. `.sdd/SKILL.md`
2. `.sdd/constitution.md`
3. `.sdd/status.md`
4. `.sdd/handoff.md` when present
5. the relevant specification and requirements

The agent must plan before implementation and validate the result against the specification.

## Source of truth

Project intent is defined by the SDD documents. Do not silently invent or change requirements.

If code, tests and specification disagree, report the conflict and resolve it explicitly.

## Completion

A task is not complete until implementation, tests, validation and documentation are updated as applicable.

Update `.sdd/status.md` after significant work and `.sdd/handoff.md` when another agent may continue the project.
