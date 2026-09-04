# SDD — Specification-Driven Development

## Purpose

This skill defines a repeatable workflow for AI-assisted software development. The specification is the source of truth for project intent, while code is its implementation.

## Workflow

READ → UNDERSTAND → PLAN → IMPLEMENT → TEST → VERIFY → DOCUMENT → HANDOFF

### 1. READ
Read `AGENTS.md`, `.sdd/constitution.md`, `.sdd/status.md`, `.sdd/handoff.md` if present, and the relevant specification/requirements.

### 2. UNDERSTAND
Identify requirements, constraints, dependencies, acceptance criteria, risks and ambiguities.

### 3. PLAN
Before significant implementation, define objective, affected requirements, files, architecture impact, tests, risks and completion criteria.

### 4. IMPLEMENT
Implement only the approved scope. Avoid unrelated refactoring. Do not silently change requirements.

### 5. TEST
Use TDD when appropriate. Add or update tests that verify behavior and important requirements.

### 6. VERIFY
Validate implementation against acceptance criteria and specification. Check regressions and relevant build/static-analysis results.

### 7. DOCUMENT
Update specifications, architecture and ADRs when decisions or intended behavior change.

### 8. HANDOFF
Update `.sdd/status.md` and `.sdd/handoff.md` when work is interrupted or another agent may continue.

## No silent decisions

If an important requirement or design choice is ambiguous:
- inspect existing project evidence;
- infer only when the inference is safe and consistent;
- otherwise document the ambiguity and request clarification.

## Traceability

Prefer the chain:

REQ → TASK → CODE → TEST → VALIDATION

Use stable IDs such as `REQ-001`, `TASK-001`, `TEST-001`.

## TDD and BDD

TDD may be used to verify implementation through automated tests.

BDD may be used to express observable behavior as Given/When/Then.

SDD, TDD and BDD are complementary:
- SDD: what must be built;
- BDD: how observable behavior is expressed;
- TDD: how implementation is automatically verified.

## Embedded software

For embedded projects explicitly consider timing, memory, power, interrupts, concurrency, watchdogs, communication protocols, fault handling, recovery, boot/reset behavior and hardware constraints when relevant.

Do not invent hardware specifications.

## Scope control

Do not introduce unrelated features, broad refactors, unnecessary dependencies or breaking API changes without justification.

## Definition of Done

A task is done only when applicable:
- requirements are identified;
- implementation is complete;
- tests are created/updated;
- tests pass;
- acceptance criteria are satisfied;
- documentation is consistent;
- status is updated;
- handoff is updated when needed.

## Required completion report

For significant work, report:

### SDD Report
- Specification
- Requirements
- Changes
- Tests
- Validation
- Decisions
- Remaining work
- Next step
