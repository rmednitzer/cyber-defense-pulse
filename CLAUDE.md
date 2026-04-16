# cyber-defense-pulse

EU cyber and defense demand-signal pulse. Weekly artifact produced by
Claude routine `cyber-defense-pulse`, Monday 06:00 UTC.

## Write paths (routine scope)

- reports/YYYY-Www.md
- reports/YYYY-Www.json
- reports/INDEX.md

## Never touch

- LICENSE
- README.md
- CLAUDE.md
- schemas/
- .gitignore
- .github/ (if created later)

## Commit policy

- Additive only. Never rewrite history.
- Commit message: `cyber-defense-pulse YYYY-Www: N items, M feed failures`
- Trailer: `Session-Id: <CLAUDE_CODE_REMOTE_SESSION_ID>`

## Artifact contract

Each weekly run produces:

1. `reports/YYYY-Www.md`: BLUF (two sentences) plus six sections
2. `reports/YYYY-Www.json`: sidecar conforming to `schemas/sidecar.schema.json`
3. `reports/INDEX.md`: prepend one row

Empty sections: heading plus `No qualifying items this week.` No padding.

## Language policy

Primary output language: English. Non-English source terms preserved in
parentheses on first use (e.g. "Verordnung (regulation)"). Priority
languages for source coverage: EN, DE, FR, IT, ES. Other EU-27
languages: title-translate only, do not synthesize content unless the
routine has verified-reliable source-language handling.

## Failure handling

- Feed returns non-200: log under "Feed health" appendix with endpoint,
  status, retry count. Do not invent content.
- Unretrievable source: refuse to summarize. Log to appendix.
- Fabrication prohibited: every factual claim must resolve to a
  retrieved URL with hash in sidecar.

## Register

Peer-engineer. No coaching tone. No marketing language. Answer-first.
