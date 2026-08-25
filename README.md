# Spaced Paste (DDU x NG) Breeding Tracker

Automated breeding-population dashboard for the **Spaced Paste (DDU x NG)** cross, ingesting live observations from the shared #breeding Discord channel and syncing to Google Drive.

- Live dashboard: https://joeydouglas.github.io/spaced-paste-breeding/
- Plant ID convention: `sp06`, `sp07`, ... (parsed from Discord text via a tightly-anchored `\bsp[\s-]?(\d{1,2})\b` pattern -- deliberately strict since "sp" is a common English substring and this channel is shared with two other crosses)
- Source of truth: `tracker.json` in the companion `~/.hermes/breeding/spaced-paste/` working directory (not this repo -- this repo holds the generated static dashboard only).

## Data provenance note

Seed data for `sp06` was extracted from the Google Doc "Spaced Paste (DDU x NG)" (1 plant, 1 observation). Two ambiguities were flagged rather than guessed at:
- The "DDU" acronym is unconfirmed; the doc text only mentions "Dulce de vale".
- The "NG" parent is assumed to be the same Nana Glue used in the Mule Fuel x Nana Glue cross (shared abbreviation + a "smells like Nana glue" note), but this has not been independently verified.

See `tracker.json`'s `notes_meta.flagged_ambiguities` for details.
