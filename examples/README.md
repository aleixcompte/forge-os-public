# Safe Public Engineering Examples

The examples in this repository intentionally demonstrate **patterns**, not production implementation.

## Example: governed action envelope

```json
{
  "goal_id": "goal-example",
  "actor": {
    "type": "agent",
    "id": "agent-example"
  },
  "requested_action": "tool.example.execute",
  "authority": {
    "scope": "example-resource"
  },
  "policy_result": "allow",
  "requires_human_approval": false
}
```

This illustrates the separation between the actor, requested capability, authority and policy result.

## Example: gated action

```text
Goal
  ↓
Policy evaluation
  ↓
Risk threshold reached
  ↓
GATE
  ↓
Human approval required
  ↓
Resume only after explicit decision
```

## Example: evidence chain

```json
{
  "execution_id": "exec-example",
  "status": "verified",
  "evidence": [
    "test-result",
    "runtime-observation"
  ],
  "checkpoint": "checkpoint-example"
}
```

These examples are intentionally generic. They reveal the engineering model without exposing production schemas, identifiers, policies or implementation.
