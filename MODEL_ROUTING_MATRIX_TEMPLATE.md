# AI Agent Model Routing Matrix Template

Use this before starting a meaningful Codex, Claude Code, Cursor, review-agent, browser-QA, or local-agent run when the model, tool, or review path is not obvious.

## Routing Decision

| Field | Value |
| --- | --- |
| Work type |  |
| Objective |  |
| Default route |  |
| Escalation trigger |  |
| Avoid rule |  |
| Verification needed |  |
| Owner |  |

## Routing Matrix

| Work Type | Default Route | Escalate When | Avoid When | Verification Needed |
| --- | --- | --- |
| Small code edit | Fast coding agent | Shared module or hidden regression risk | Requirements are unclear | Focused test or diff check |
| Cross-file refactor | Strong coding model | Public API, schema, or state flow changes | No test coverage exists | Full relevant test slice |
| UI change | Frontend agent plus browser QA | Responsive layout or visual state is risky | No running app is available | Screenshot or browser check |
| Code review | Review agent | Security, data, payment, auth, or migration risk | The diff is not stable | File and line findings |
| Research / docs | Browser-capable agent | Current API, pricing, legal, or policy facts matter | Offline recall is enough | Source links and date |
| Release / revenue claim | Verification-first agent | Money, delivery, or public release is involved | Payment evidence is missing | Receipt, dashboard, digest, or release evidence |

## Model Choice Rule

Use the cheapest reliable route that can produce direct proof.

Escalate only when at least one is true:

- The run touches shared behavior.
- The run changes release, payment, auth, or buyer-facing surfaces.
- A previous run failed for weak reasoning or missing context.
- Verification requires multiple tools or rendered output.
- The cost of a wrong answer is higher than the model-cost difference.

## Buyer Request Packet

Use these exact lines when requesting the team license:

```text
Invoice request packet: Agent Ops Command Center
Request package: Team license - 7 seats - $203 gross
Need: AI-agent model routing templates for model selection, escalation rules, review paths, verification gates, and cost control.
Proof rule: Count revenue only after checkout, receipt, payout, or seller-dashboard evidence.
```

Primary $203 team request URL:

https://ivelly42.github.io/agent-ops-command-center/team-request-url.html

Checkout status:

https://ivelly42.github.io/agent-ops-command-center/checkout-status.json

Invoice request packet:

https://ivelly42.github.io/agent-ops-command-center/team-invoice-request.html

## Revenue Rule

Model-routing interest is not revenue.

Count revenue only when checkout, receipt, payout, or seller-dashboard evidence proves payment.
