# CITY-PULSE — T2 Software Metrics + System Quality Package

This package is prepared for the `t2-metrics` branch.

## Files

- `docs/gqm-plan.md` — completed T2 Goal–Question–Metric plan.
- `docs/metrics-report.md` — evidence-based T2 report draft.
- `docs/defect-log.md` — observed issues and their evidence/status.
- `docs/system-quality-dashboard.md` — implementation specification for the System Quality section.
- `docs/evidence/known-results.md` — results already obtained from project tool/log runs.
- `docs/evidence/metrics-evidence.json` — machine-readable evidence ledger.
- `scripts/t2-code-metrics.js` — repository scanner for LOC, comments, duplication and complexity indicators.
- `scripts/t2-system-quality.js` — log summarizer for provider quality and reading-state percentages.
- `scripts/t2-run.ps1` — Windows helper to run the T2 evidence scripts.
- `dashboard/system-quality-section.html` — drop-in System Quality dashboard section. It is intentionally standalone because the source `project_citypulse.html` was not available in this workspace.

## Important evidence rule

The team plan says every reported number must trace to a provider, documented formula, authority-approved notice, or labelled scenario. This package therefore does **not** invent missing values. Where a value requires a repository/log run that is not present in the available workspace, it is marked `PENDING REPOSITORY RUN`.

## Current verified evidence included

- Test suite: 30/30 checks passed (100%).
- ESLint/code analysis: 4 warnings, 0 errors.
- `createServer` complexity: 16.
- Async function complexity: 59.
- Two async-arrow complexity findings: 22 each.
- Notices: 112 fetches, 84.8% success, p50 13 ms, p95 46 ms.
- Traffic: 29 fetches, 0% success because `TOMTOM_API_KEY` was not configured during the run.
- Weather: 18 fetches, 100% success, p50 705 ms, p95 2339 ms.
- Air Quality: 16 fetches, 100% success, p50 916 ms, p95 1594 ms.
- No data gaps were reported by the log analysis run.

These values are recorded as previously obtained project evidence; re-run the supplied scripts against the current branch before final submission so the evidence reflects the final repository state.
