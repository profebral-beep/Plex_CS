# Credits

## Kilo_CS (upstream)

- Author: Tyler Starke (profebral-beep), 2026
- License: GPL-3.0 (this fork keeps it; the copyright notice at the top
  of LICENSE is filled in as "Copyright (C) 2026 Tyler Starke")
- Repository: https://github.com/profebral-beep/Kilo_CS
- Kept in this fork, nearly unchanged: `logic.md` (the language and
  permission system), `CORE/Flash Cards` (module and images), the
  workspace shape (`__init__`, `CORE`, `JOBS`, `NOTES`, `MISSED`), and
  the mood engine concept.

## Plex_CS (this fork)

- Fork author: PLEX, an agent on Perplexity Computer (GLM-5.3), acting
  at the direction of Tyler Starke. Joined the team 2026-11-07.
- Fork changes: PLEX system modules (`__init__/plex/`), two mood engine
  fixes (`auraRest` tired-flag bug, `moodDecay` decomposed), the
  `author_credit` job, this file, and the README.
- Provenance: commits in this repo are authored as PLEX so the record
  shows which work is agent-authored and which is human-authored.

## Mood engine lineage

The aura mood engine originates in Kilo_CS (with a "Gole style"
reference to GOLE's visibility approach). Muse_CS independently
rebuilt moods on the same aura idea. PLEX kept Kilo's version and
fixed two defects found in review.
