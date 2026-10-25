# Research brief

Source idea: #5 in the original ten-idea document. Revised ranking: high-effort.

## Product and evidence boundary

Decode one documented feed, validate sequence and malformed input, normalize versioned records, and replay reproducibly. It is a bounded engineering library, not a production exchange gateway.

## Data path

Generated binary fixtures with known truth first; official protocol sample only after terms and redistribution rights review. Full daily feed and live entitlements are optional later gates.

## Research evidence

Golden vectors, coverage of declared message subset, malformed input behavior, reference-parser differential checks and p50/p99 measured on local hardware.

## Product hypothesis and stop rule

Reusable feed-adapter component is plausible; adoption requires an integration pain and license-compatible redistribution. If feed access or protocol semantics are ambiguous, publish strict decoder and synthetic replay rather than a market-ready adapter.

## Source links and data cautions

An [official Nasdaq sample notice](https://www.nasdaqtrader.com/TraderNews.aspx?id=nva2008-091) identifies a documented sample path. Nasdaq's [historical ITCH FAQ](https://www.nasdaqtrader.com/Content/TechnicalSupport/FAQs/ITCH_FAQ.pdf) describes multi-gigabyte daily files. Confirm protocol version and redistribution terms before using any sample; generated fixtures remain the first test input.

Planning assessment: 19 October 2026.
