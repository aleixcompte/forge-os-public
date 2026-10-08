# Engineering Principles

FORGE OS follows a governance-first engineering method.

## Capability is not authority

A system being technically able to perform an action does not mean it is authorized to do so.

```text
Capability ≠ Authority
```

## Evidence before status

Terms such as:

- tested
- committed
- deployed
- verified
- complete

should only be used when supporting evidence exists.

## Inspect before build

Preferred sequence:

```text
Discovery
→ Verify
→ Plan
→ Minimal Change
→ Tests
→ Evidence
→ Review
→ Deploy Plan
→ Approval when required
→ Apply
→ Verify
→ Checkpoint
```

## Persist milestones, not noise

Durable state should preserve information needed to resume and govern work, not every conversational detail.

## Reversibility

Material changes should have:

- known impact
- bounded scope
- rollback strategy
- verification after application

## Least privilege

Agents, tools and services should receive only the authority needed for the current task.

Delegation must never increase authority beyond that of the delegating actor.

## Provider independence

Models and external services should remain replaceable where practical.

## Human control

FORGE should execute what has been authorized and stop where policy requires a human decision.
