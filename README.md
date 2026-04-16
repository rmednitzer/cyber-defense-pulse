# cyber-defense-pulse

Weekly analytical pulse on EU cyber and defense signals. Produced every
Monday 06:00 UTC, one artifact per ISO week.

## Scope

Six sections per weekly artifact:

1. Regulatory implementation (NIS2, CRA, AI Act, DORA, ENISA guidance,
   Commission acts)
2. Operational advisories (CSIRTs Network, ENISA, CERT-EU, national
   CSIRT cross-border output)
3. Legislative motion (European Parliament ITRE, LIBE, SEDE, IMCO;
   Council; trilogue outcomes)
4. Defense procurement demand signal (TED CPV 72/35/73 all member
   states, EDF, EDIP, PESCO, EDA, ASAP, SAFE)
5. Data protection decisions (EDPB, national DPAs)
6. Calendar deltas (EDF, EDIP, CEF Digital, CRA, AI Act, NIS2
   transposition)

Empty sections retained with explicit "No qualifying items this week."
No padding.

## Artifact contract

Each weekly run produces three files:

- `reports/YYYY-Www.md`, human-readable pulse with two-sentence BLUF
- `reports/YYYY-Www.json`, machine-readable sidecar per `schemas/`
- `reports/INDEX.md`, prepended row with item count and feed health

Example: `reports/2026-W17.md`

## Sources

Primary sources only. Every cited item includes publisher, publication
date, retrieval timestamp, and SHA-256 content hash in the sidecar JSON.
Non-English content: verbatim terms preserved in parentheses on first
use, translation follows.

## Methodology

Automated synthesis via scheduled Claude routine. Author reviews for
accuracy. Corrections committed additively without history rewrites.
Failure handling: unretrievable sources logged in "Feed health"
appendix, not paraphrased from memory. No speculation on legislative
outcomes.

## Disclaimer

Analytical synthesis, not legal advice. Not affiliated with any EU
institution, member state agency, or private entity cited.
Interpretations are the author's.

## Author

Roman Mednitzer, Vienna.
Senior Systems Engineer and Assurance Architect.
https://rmednitzer.github.io

## License

Licensed under the Apache License, Version 2.0. See [LICENSE](./LICENSE).
