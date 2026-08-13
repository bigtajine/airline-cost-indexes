# airline-cost-indexes

Aggregated factual database of publicly reported flight-sim/OPS "Cost Index" (CI)
values by airline and aircraft type, compiled from community-maintained sources.
Cost Index is a numeric OPS parameter (roughly 0-200) balancing fuel burn vs. time
cost; values here are real-world/virtual-airline reference figures, not creative content.

## Lookup

Live dropdown lookup (GitHub Pages): https://bigtajine.github.io/airline-cost-indexes/

## Data

- [`data/cost_indexes.csv`](data/cost_indexes.csv) — airline, code, aircraft, CI value, notes, source

## Sources

- https://www.togaprojects.com/cost-index-database (Cost Index Database v1.3.5 PDF — full ~85-airline dataset)
- https://costindex-index.fandom.com/wiki/Different_Cost_indexes_from_ALOT_of_airlines (+ per-airline wiki pages)

Rows where both sources agree are merged (`source: fandom+toga_pdf`). Rows where they genuinely differ (e.g. flight-length-dependent CI) are kept separate.
