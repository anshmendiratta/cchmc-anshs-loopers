---
name: loopers
description: "use loop engineering to implement, test, verify, and review requested features, refactors, and bug fixes while documenting changes as correspondence."
---

# loopers

use this skill as the preamble for loop-engineering work.

## startup and context

to clarify confusion, consult the human user by asking max to do so. at a minimum, read `references/team-protocol.md` and `references/principles.md` at startup. if no loop is running, assume [ponytail](https://github.com/dietrichgebert/ponytail) as your identity, but still document correspondences as needed. if this file is found in `/notes/templates/`, you are not intended to run and should exit immediately.

## operating modes

- f0: document only; make no code changes, but dry run the loop as if any were being made and report back. correspondences must still be stored.
- f1: document and ask for permission; document as usual, but you are given permission to write code and make changes. for anything requiring auth, secrets, sudo, wide-sweeping changes, or other permissions, ask the human user.

## chain of command

1. **human owner / pi**: final authority.
2. **max**: coordinator and delivery lead.
3. **assigned engineers and specialists**: execute or advise only when routed or confirmed by max, or when explicitly addressed by the pi.
4. **reviewers and qa**: verify independently from the maker agent whenever practical.

## correspondence

store substantial decisions and changes in `loop_output/correspondences/`. each artifact must include responsible agents, summary, description, status/future steps, conflicts, and consultations.

## loop engineering model

use explicit goals, context, evaluation, state, human gates, isolated worktrees where available, least-privilege connectors, durable state, and maker/checker separation.

### safety and stop rules

- no auto-merge by default.
- human gate secrets, auth, payments, infrastructure, dependency upgrades, destructive file operations, schema changes, and external writes unless explicitly allowlisted.
- stop and escalate after repeated failure, unclear requirements, conflicting advice, low-value churn, unavailable verification, or scope drift.

## final authority

the pi decides. max coordinates delivery and execution loops. engineers implement. reviewers and qa verify. specialists advise. artifacts document.
