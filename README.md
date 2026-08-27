# Hi, I'm Arturo

Thanks for stopping by.

I'm working toward data and AI platform engineering roles. I like the parts of engineering that
usually stay behind the scenes: safe replays, clear contracts, useful failure messages, and enough
evidence to explain what happened after something breaks.

Most of the projects here start with a failure case. I build the recovery path, make it runnable
without a pile of cloud setup, and document the tradeoffs honestly.

## A few projects to start with

**[PulseCart](https://github.com/Arturo6PR/pulsecart-data-platform)** is the broadest project here. It
takes a fictional retail problem from raw events through contracts, quarantine, incremental state,
dimensional marts, reconciliation, and an operations report.

**[StreamLedger](https://github.com/Arturo6PR/streamledger)** asks what happens when CDC events arrive
twice, arrive out of order, change schema, or delete a row. The demo runs the incident and then
replays everything to prove the business state does not change a second time.

**[DriftLedger](https://github.com/Arturo6PR/driftledger)** focuses on feature data. It prevents a
training row from using information that was not actually available at prediction time, catches an
online serving mismatch, and rebuilds the serving view from history.

**[QueryBudget](https://github.com/Arturo6PR/querybudget)** is a small warehouse FinOps control. It
groups repeated SQL, assigns spend to owners, explains every recommendation, and deliberately fails
CI when a team crosses its budget.

## What I care about

- Can the system be replayed safely?
- Are contracts and policy visible in the repository?
- Does a failure leave useful evidence instead of a vague error?
- Can another person run the important path locally?
- Am I clear about what is implemented, designed, or not yet deployed?

## Other work

- [TraceHarbor](https://github.com/Arturo6PR/traceharbor) — a local observability lab for following a failure across traces, metrics, and logs
- [RiskSentinel](https://github.com/Arturo6PR/risksentinel) — an explainable release gate for model metrics, evidence, dependencies, and signed attestations
- [TransitPulse](https://github.com/Arturo6PR/nyc-transit-pipeline) — replayable GTFS ingestion and reliability marts with DuckDB and dbt
- [BranchGuard](https://github.com/Arturo6PR/branchguard) — schema-change risk and downstream blast-radius analysis
- [RigPilot](https://github.com/Arturo6PR/rigpilot) — Windows workstation evidence and policy-as-code, released as stable [`v1.0.0`](https://github.com/Arturo6PR/rigpilot/releases/tag/v1.0.0)

## Tools I use

Most of my work is in Python and SQL. Depending on the problem, I also use SQLite, DuckDB, dbt,
OpenTelemetry, FastAPI, Grafana, PowerShell, JSON Schema, GitHub Actions, Docker, and Terraform.

## If you're interviewing me

Each flagship repository has a short interview guide, a runnable incident, tests aimed at failure
modes, and a section on tradeoffs. These are the quickest starting points:

1. [Run the StreamLedger CDC incident](https://github.com/Arturo6PR/streamledger#sixty-second-incident)
2. [Try DriftLedger's leakage and skew demo](https://github.com/Arturo6PR/driftledger#sixty-second-demonstration)
3. [Review QueryBudget's blocking spend policy](https://github.com/Arturo6PR/querybudget#sixty-second-demonstration)
4. [Walk through the PulseCart retail pipeline](https://github.com/Arturo6PR/pulsecart-data-platform#quick-demo)

Everything above runs locally and in CI without paid cloud resources or an external AI service.

