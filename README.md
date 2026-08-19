# 16 — Risk / Compliance

> Part of the **Hermes Organizational Decision System**. This repo is the
> **Risk / Compliance** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/hermes-ios/00-kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> What constraints and risks must we manage before they become material failures?

## Purpose
Identify, assess, mitigate, and monitor risk and compliance obligations.

## Sub-functions
Enterprise Risk, Compliance Monitoring, Controls Testing, Regulatory Change, Third-Party Risk, Incident & Breach Management

## Typical roles
Chief Risk Officer, VP Compliance, Risk Director, Compliance Manager, Controls Auditor

## Inputs
Obligations, controls, incidents, metrics, regulatory changes, assurance evidence.

## Outputs
Risk assessments, control validations, compliance attestations, remediation, risk appetite decisions.

## Learning focus
Leading indicators; control effectiveness; compliance failures; risk concentrations; regulatory trends.

## Operating tree
```text
OBLIGATION / RISK →
    ASSESSMENT →
    CAUSE →
    PROBABILITY →
    IMPACT →
    CONTROLS →
    CONTROL EFFECTIVENESS →
    EARLY SIGNALS →
    RESPONSE →
    ACCEPTABLE RISK →
    MITIGATION →
    MONITORING
```

## Decision states
```text
IDENTIFIED → ASSESSED → CONTROLLED → MONITORED → BREACHED → REMEDIATING → CLOSED
```

## Decision outputs
`Accept · Mitigate · Transfer · Avoid · Escalate · Monitor`

## Critical prompts (what this function thinks about)
> What risk or obligation exists?
> What is the cause?
> What is the probability?
> What is the impact?
> What controls exist?
> Are they effective?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/16-risk-compliance.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
