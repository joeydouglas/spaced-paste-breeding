# Spaced Paste (Dulce de Uva x Nana Glue) — Breeding Data Repo

**Record of truth** for the **Spaced Paste (Dulce de Uva x Nana Glue)** breeding cross,
in markdown. Observations arrive from the shared #breeding Discord channel and are committed
here automatically.

## Layout

| Path              | Meaning                                            |
| ----------------- | -------------------------------------------------- |
| `project.md`      | Cross-level record: parents, roster, project notes  |
| `plants/<ID>.md`  | One file per plant — the plant's full record        |

These are the only files the breeding data API reads; anything else in this repo is ignored.

- Plant ID convention: `sp01`, `sp02`, ... (parsed from Discord text via a tightly-anchored
  `\bsp[\s-]?(\d{1,2})\b` pattern — deliberately strict, since "sp" is a common English
  substring and the #breeding channel is shared with other crosses)
- Legacy generated dashboard (HTML/CSS): https://github.com/joeydouglas/spaced-paste-dashboard-legacy

## History

This repo previously held **both** the markdown data and the generated static dashboard.
The dashboard was split out into `joeydouglas/spaced-paste-dashboard-legacy`; this repo is
now data-only. No history was rewritten — the dashboard files were removed in an ordinary
commit and remain reachable in this repo's history.

## Provenance note

Seed data for `sp06` was extracted from the Google Doc "Spaced Paste (DDU x NG)". Two
ambiguities were confirmed by Joey (2026-08-25):

- **DDU = Dulce de Uva** (confirmed).
- **NG parent = the same Nana Glue** used in the Mule Fuel x Nana Glue cross (confirmed).
