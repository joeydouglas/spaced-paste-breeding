# Spaced Paste (Dulce de Uva x Nana Glue) Breeding Tracker

Automated breeding-population dashboard for the **Spaced Paste (Dulce de Uva x Nana Glue)** cross, ingesting live observations from the shared #breeding Discord channel and syncing to Google Drive.

- Live dashboard: https://joeydouglas.github.io/spaced-paste-breeding/
- Plant ID convention: `sp06`, `sp07`, ... (parsed from Discord text via a tightly-anchored `\bsp[\s-]?(\d{1,2})\b` pattern -- deliberately strict since "sp" is a common English substring and this channel is shared with two other crosses)
- Source of truth: `tracker.json` in the companion `~/.hermes/breeding/spaced-paste/` working directory (not this repo -- this repo holds the generated static dashboard only).

## Data provenance note

Seed data for `sp06` was extracted from the Google Doc "Spaced Paste (DDU x NG)" (1 plant, 1 observation). Two ambiguities were flagged and have since been confirmed by Joey (2026-08-25):
- **DDU = Dulce de Uva** (confirmed).
- **NG parent = the same Nana Glue** used in the Mule Fuel x Nana Glue cross (confirmed).

No explicit keeper/culled status was found for `sp06` in the source doc, so its status remains `active` pending further observation.

See `tracker.json`'s `notes_meta.resolved_ambiguities` for details.
