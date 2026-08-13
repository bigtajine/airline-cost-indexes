# airline-cost-indexes

Aggregated factual database of publicly reported flight-sim/OPS "Cost Index" (CI)
values by airline and aircraft type, compiled from community-maintained sources.
Cost Index is a numeric OPS parameter (roughly 0-200) balancing fuel burn vs. time
cost; values here are real-world/virtual-airline reference figures, not creative content.

## Lookup

Live dropdown lookup (GitHub Pages): https://bigtajine.github.io/airline-cost-indexes/

## Data

- [`data/cost_indexes.csv`](data/cost_indexes.csv) — airline, code, aircraft (ICAO type designator), CI value, notes

Aircraft types follow the [ICAO type designator list](https://en.wikipedia.org/wiki/List_of_aircraft_type_designators)
(`B738` = 737-800, `A332` = A330-200, etc.) so the same type from different
sources always lines up under one row instead of duplicating.

CI value formats:
- `20` — single value
- `10-20` — range
- `9/8` — discrete alternatives (e.g. outbound/inbound)
- `50(250)` — base value, delayed-ops value in parentheses

Compiled from the TOGA Projects Cost Index Database PDF and the
costindex-index fandom wiki. Where the two sources agreed, they were merged
into one row; where they genuinely conflicted (e.g. flight-length-dependent
CI), both values are kept as separate rows.
