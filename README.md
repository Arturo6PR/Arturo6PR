# Hi, I'm Arturo

I build reliable data systems and deterministic tools for platform engineering, data governance,
and safe AI-model delivery. My current focus is Data/AI Platform Engineering and Cloud/Platform
Engineering: replayable pipelines, explicit policy, reproducible automation, and security
boundaries that are easy to audit.

## Featured projects

| Project | What it does | Engineering focus |
| --- | --- | --- |
| [TransitPulse](https://github.com/Arturo6PR/nyc-transit-pipeline) | Replays GTFS-Realtime feeds into an idempotent analytical store and summarizes transit reliability | Python, DuckDB, protobuf, data quality, deterministic ingestion |
| [RigPilot](https://github.com/Arturo6PR/rigpilot) | Turns read-only Windows workstation evidence into deterministic assessments and CI policy decisions | Python, PowerShell, JSON Schema, policy-as-code, GitHub Actions |
| [BranchGuard](https://github.com/Arturo6PR/branchguard) | Detects risky schema changes and calculates their transitive downstream blast radius | Data contracts, graph traversal, Docker, CI, Terraform and AWS design |
| [RiskSentinel](https://github.com/Arturo6PR/risksentinel) | Evaluates AI-model release risk from metrics, evidence, dependencies, and optional signed attestations | MLOps governance, Ed25519, offline MLflow interoperability, reusable actions |

[![TransitPulse CI](https://github.com/Arturo6PR/nyc-transit-pipeline/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/nyc-transit-pipeline/actions/workflows/ci.yml)
[![RigPilot CI](https://github.com/Arturo6PR/rigpilot/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/rigpilot/actions/workflows/ci.yml)
[![BranchGuard CI](https://github.com/Arturo6PR/branchguard/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/branchguard/actions/workflows/ci.yml)
[![RiskSentinel CI](https://github.com/Arturo6PR/risksentinel/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Arturo6PR/risksentinel/actions/workflows/ci.yml)

### TransitPulse

A local-first GTFS-Realtime pipeline that preserves raw protobuf payloads, normalizes trip-stop and
service-alert records, prevents duplicate ingestion with content-derived identities, and produces
route-delay analytics from an embedded DuckDB store. Its offline fixture makes the full workflow
reproducible without transit credentials or cloud resources.

### RigPilot

Windows-first workstation intelligence with explicit read-only collection, strict versioned JSON
contracts, pure assessment and policy engines, stable exit codes, and a reusable GitHub Action.
RigPilot has reached stable [`v1.0.0`](https://github.com/Arturo6PR/rigpilot/releases/tag/v1.0.0).

### BranchGuard

A local-first schema change gate that classifies changes as `SAFE`, `WARNING`, or `BREAKING`, then
reports `PASS`, `WARN`, or `FAIL` with cycle-safe dependency impact. Its AWS and Terraform assets
are validated infrastructure designs and have not been deployed.

### RiskSentinel

An explainable AI-model release gate that produces `APPROVE`, `REVIEW`, or `BLOCK`. It supports
direction-aware metric policy, required evidence, dependency impact, detached Ed25519 attestations,
and deterministic conversion of offline MLflow run exports without contacting a live platform.

## How I build

- Versioned contracts before integrations
- Deterministic outputs suitable for CI and audit
- Clear separation between policy outcomes and operational failures
- Behavior-focused tests across supported operating systems
- Least-privilege automation with documented trust boundaries
- Honest scope: validated designs are not presented as running deployments

## Core toolkit

`Python` · `DuckDB` · `GTFS-Realtime` · `PowerShell` · `pytest` · `Ruff` · `JSON Schema` ·
`GitHub Actions` · `Docker` · `Terraform` · `AWS architecture` · `Policy-as-code` ·
`Graph algorithms` · `Ed25519`

## Start here

1. [TransitPulse's replayable GTFS-Realtime quickstart](https://github.com/Arturo6PR/nyc-transit-pipeline#quick-start)
2. [BranchGuard's 60-second schema-risk demo](https://github.com/Arturo6PR/branchguard#60-second-demo)
3. [RiskSentinel's AI-model release demo](https://github.com/Arturo6PR/risksentinel#60-second-demonstration)
4. [RigPilot's five-minute deterministic demo](https://github.com/Arturo6PR/rigpilot#five-minute-quickstart)

All four projects run locally and in CI without requiring a cloud deployment or an external AI
service.
