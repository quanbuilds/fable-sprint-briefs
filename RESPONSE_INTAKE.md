# Response Intake

## Workflow

1. Quan sends one prompt from `DAY_1_CALLS.md` or `DAY_2_CALLS.md` to the Google Voice number connected to Fable 5.
2. Quan forwards Fable's response to Botler.
3. Botler removes secrets/private client details, saves the response under `responses/day-1/` or `responses/day-2/`, and updates the synthesis.
4. The next Fable call may reference the public response folder.
5. Botler routes implementation: Cash for lead/revenue assets, Dev for code/site work, Jim for F10.0RD.

## Naming

- `responses/day-1/01-signallabs-conversion-teardown.md`
- `responses/day-1/02-gym-icp-wedge.md`
- Continue by call number and short topic.

## Intake header

```markdown
# Fable Response — <topic>

- Day/call:
- Received:
- Source prompt:
- Public-safe review: pending
- Implementation owner:
- Status: received_not_verified

## Response

<paste response>

## Botler verification

- Claims checked:
- Conflicts:
- Decision:
- Next artifact:
```

## Rules

- Fable output is advice, not verified ground truth.
- Do not publish claims, pricing guarantees, legal language, security claims, or integrations without verification.
- Do not commit private phone numbers, lead lists, access details, or customer data.
- Every response must end in an owned implementation action or be marked rejected/deferred.
