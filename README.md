# airline-cost-indexes

Aggregated factual database of publicly reported flight-sim/OPS "Cost Index" (CI)
values by airline and aircraft type, compiled from community-maintained sources.
Cost Index is a numeric OPS parameter (roughly 0-200) balancing fuel burn vs. time
cost; values here are real-world/virtual-airline reference figures, not creative content.

## Lookup

Live dropdown lookup (GitHub Pages): https://bigtajine.github.io/airline-cost-indexes/

## Data

- [`data/cost_indexes.csv`](data/cost_indexes.csv) — airline, code, aircraft, CI value, notes, source (466 rows, sorted by airline/aircraft)

## Sources

- https://www.togaprojects.com/cost-index-database (Cost Index Database v1.3.5 PDF — full ~85-airline dataset)
- https://costindex-index.fandom.com/wiki/Different_Cost_indexes_from_ALOT_of_airlines (+ per-airline wiki pages)
- https://es.scribd.com/document/412889192/Airlines-Cost-Index-Database (partial — Scribd gates full-document text behind login/paywall)
- https://www.scribd.com/document/493346746/Cost-Index-Database (metadata only — full content paywalled, not extracted)
- https://skyteamvirtual.org/fleet/types

## Notes

- Scribd sources could only be partially retrieved (preview text); values marked `source: scribd` come from what was accessible without a paid/authenticated session.
- Several entries have duplicate airline/aircraft rows across sources with differing values — both are kept with distinct `source` and `notes` so provenance is preserved instead of guessing which is authoritative.
