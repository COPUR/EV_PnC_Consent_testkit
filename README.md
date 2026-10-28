# EV_PnC_Consent_testkit

End-to-end and conformance tests: Gherkin acceptance, revocation SLA test, PDP load test, DAST.

Part of the **EV Owners Roaming Consent** project: a central, neutral consent registry and decision point for EV owners' roaming data (which hub may receive which data, for which purpose, under which KVKK safeguard). Repo family plan: `repo-plan/consent/README.md` in the project files.

## Scope

- Gherkin features from `roaming-consent/acceptance/` (31 requirements)
- Revocation → token invalid at hub ≤ 15 min test using EV_PNC_simulator hub mocks
- k6/Gatling load tests for the PDP
- Security tests in CI (DAST, dependency scan)

## Requirements

all (verification) (see `EV_PnC_Consent_docs`, specs from `roaming-consent/spec.md`)

## Tech stack

Java + Cucumber, k6, OWASP ZAP

## Infrastructure (BOM)

Ephemeral test namespace

## Scaling

Runs per pull request (fast suite) and nightly (full + load)

## Ownership

QA · Visibility: public · Wave 1: now (Phase 0–1, Nov 2026 – Feb 2027)

## Status

Scaffold only. Not production ready.

## License

Apache-2.0 (proposed)
