# Hi, I'm Arturo

I build reliable data systems and deterministic tools for platform engineering, data governance,
and safe AI-model delivery. My current focus is Data/AI Platform Engineering: replayable pipelines,
explicit policy, reproducible automation, and security boundaries that are easy to audit.

## Platform reliability portfolio

These projects cover one operating story: ingest trustworthy data, preserve correctness under
failure, observe the system, control cost, and release models with evidence.

| Project | What it proves | Engineering focus |
| --- | --- | --- |
| [PulseCart](https://github.com/Arturo6PR/pulsecart-data-platform) | Builds a replay-safe retail pipeline from contracts through dimensional marts and an operations report | Data engineering, SQLite, SQL, incremental state, reconciliation |
| [StreamLedger](https://github.com/Arturo6PR/streamledger) | Prevents duplicate, reordered, deleted, and incompatible CDC events from corrupting serving state | CDC semantics, idempotency, source ordering, quarantine, recovery |
| [DriftLedger](https://github.com/Arturo6PR/driftledger) | Blocks temporal leakage and detects then repairs online/offline feature skew | Point-in-time joins, feature lineage, freshness SLOs, AI platform |
| [TraceHarbor](https://github.com/Arturo6PR/traceharbor) | Makes local distributed-system failures visible with correlated telemetry | OpenTelemetry, FastAPI, Grafana, observability, incident analysis |
| [QueryBudget](https://github.com/Arturo6PR/querybudget) | Converts warehouse query history into owned budgets and explainable optimization evidence | SQL fingerprints, FinOps, policy-as-code, CI enforcement |
| [RiskSentinel](https://github.com/Arturo6PR/risksentinel) | Gates AI-model releases with metrics, evidence, dependency impact, and signed attestations | MLOps governance, Ed25519, MLflow interoperability, reusable actions |

[![PulseCart CI](https://github.com/Arturo6PR/pulsecart-data-platform/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/pulsecart-data-platform/actions/workflows/ci.yml)
[![StreamLedger CI](https://github.com/Arturo6PR/streamledger/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/streamledger/actions/workflows/ci.yml)
[![DriftLedger CI](https://github.com/Arturo6PR/driftledger/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/driftledger/actions/workflows/ci.yml)
[![QueryBudget CI](https://github.com/Arturo6PR/querybudget/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/querybudget/actions/workflows/ci.yml)

### PulseCart

An interview-ready retail data platform with versioned contracts, quarantine, replay-safe
incremental processing, dimensional marts, reconciliation, quality evidence, and a business-facing
operations report.

### StreamLedger

A CDC correctness lab that stores durable event identity separately from source position. Its
incident demo proves a full replay makes zero extra mutations while stale changes and unsupported
schemas remain auditable.

### DriftLedger

A feature data platform that uses both observation time and availability time for training joins.
It records feature lineage, detects an injected serving mismatch, and rebuilds online state from
immutable offline history.

### QueryBudget

A vendor-neutral warehouse FinOps analyzer with stable SQL fingerprints, explicit team budgets,
named optimization rules, conservative non-additive savings estimates, and a blocking CI policy.

### TraceHarbor

A local distributed-systems observability lab that correlates traces, metrics, and logs so an
interviewer can move from a symptom to a concrete failing dependency.

### RiskSentinel

An explainable AI-model release gate that produces `APPROVE`, `REVIEW`, or `BLOCK` from metrics,
required evidence, dependency impact, and optional signed attestations.

## Additional engineering projects

- [TransitPulse](https://github.com/Arturo6PR/nyc-transit-pipeline) — replayable GTFS ingestion and tested reliability marts with DuckDB and dbt
- [BranchGuard](https://github.com/Arturo6PR/branchguard) — deterministic schema-change risk and downstream blast-radius analysis
- [RigPilot](https://github.com/Arturo6PR/rigpilot) — Windows workstation evidence and policy-as-code, released as stable [`v1.0.0`](https://github.com/Arturo6PR/rigpilot/releases/tag/v1.0.0)

## How I build

- Versioned contracts before integrations
- Deterministic outputs suitable for CI and audit
- Clear separation between policy outcomes and operational failures
- Behavior-focused tests across supported operating systems
- Least-privilege automation with documented trust boundaries
- Honest scope: validated designs are not presented as running deployments

## Core toolkit

`Python` · `SQL` · `SQLite` · `DuckDB` · `dbt` · `OpenTelemetry` · `FastAPI` · `Grafana` ·
`PowerShell` · `JSON Schema` · `GitHub Actions` · `Docker` · `Terraform` · `AWS architecture` ·
`CDC semantics` · `Feature data` · `FinOps` · `Policy-as-code` · `Ed25519`

## Start here

1. [StreamLedger's deterministic CDC incident](https://github.com/Arturo6PR/streamledger#sixty-second-incident)
2. [DriftLedger's temporal-leakage and skew demonstration](https://github.com/Arturo6PR/driftledger#sixty-second-demonstration)
3. [QueryBudget's blocking warehouse-spend review](https://github.com/Arturo6PR/querybudget#sixty-second-demonstration)
4. [PulseCart's replay-safe retail demo](https://github.com/Arturo6PR/pulsecart-data-platform#quick-demo)
5. [TraceHarbor's distributed-systems lab](https://github.com/Arturo6PR/traceharbor)

The featured projects run locally and in CI without requiring paid cloud resources or an external
AI service.

