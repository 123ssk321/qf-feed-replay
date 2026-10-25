# Feed Replay C++ execution plan

Prepared 2026-10-25. **Queued; implementation inactive.** Original idea #5.

## Product contract

Decode one documented feed, validate sequence and malformed input, normalize versioned records, and replay reproducibly. It is a bounded engineering library, not a production exchange gateway.

## Architecture and data

Generated binary fixtures with known truth first; official protocol sample only after terms and redistribution rights review. Full daily feed and live entitlements are optional later gates. Version inputs and generated seeds. Separate ingestion/generation, domain model, evaluation and public interface. First measure a bounded local run; paid data and cloud compute are outside this plan.

## Evaluation contract

Golden vectors, coverage of declared message subset, malformed input behavior, reference-parser differential checks and p50/p99 measured on local hardware. Prespecify baselines, data splits and failure categories before final evaluation. Record exact commands, resource measurements, all tried variants and negative results. Simulated evidence remains separate from real-market or user validation.

## Milestones and hours

Months are relative to future activation. First public functional result: month 3; final decision: by month 12. One candidate uses the shared 16-hour weekly capacity, never six concurrent commitments. Total 420 hours includes 120 reserve.

| Milestone | Relative window | Task hours | Reserve | Cumulative |
| --- | --- | ---: | ---: | ---: |
| QF-M1: Protocol and fixture contract | Months 1–2 | 50 | 20 | 70 |
| QF-M2: Decoder and normalizer slice | Months 1–2 | 50 | 20 | 140 |
| QF-M3: First public replay artifact | Month 3 | 50 | 18 | 208 |
| QF-M4: Sequence and fault recovery | Months 5–7 | 50 | 22 | 280 |
| QF-M5: Profiling and integration | Months 6–8 | 50 | 20 | 350 |
| QF-M6: Stable library and adoption decision | Months 7–12 | 50 | 20 | 420 |

## Public result and release gate

At milestone 3 publish a runnable artifact, generated or permitted inputs, correctness checks, a baseline, exact run instructions and an honest limitations report. This planning repository is not that artifact. A later stable release needs reproducible evaluation, failure evidence, bounded resource use and a named user workflow.

## Product decision

Reusable feed-adapter component is plausible; adoption requires an integration pain and license-compatible redistribution. If feed access or protocol semantics are ambiguous, publish strict decoder and synthetic replay rather than a market-ready adapter. At each milestone decide continue, narrow or park using actual hours and evidence. No recurring monitor, spending, live trading, conference submission or implementation is activated by this plan.
