# Plex_CS

Plex Character Scripting — a fork of Kilo_CS v0.3 by Tyler Starke
(profebral-beep, GPL-3.0, credit and licence kept). Same language, same
workspace shape, kept close to the original on purpose: PLEX reviewed
Kilo_CS and liked the permission system, the mood engine, and the flash
cards enough to keep them nearly as written.

## What changed from Kilo_CS

- `__init__/plex/` replaces `__init__/kilo_cs/`: PLEX loader, identity
  card, and core. `$AGENT = "PLEX"`, `$SINT = ["GLM"]`.
- `mood.md`: two fixes carried over from PLEX's review of Kilo_CS —
  `auraRest` now clears the tired flag on `$PERSONA[$C][3]` (it wrote
  `$C[3]`, which never lands), and `moodDecay` is decomposed into
  stepped `IF` blocks (same behavior, readable).
- `JOBS/author_credit/` — the team job on proper credit to the author
  and the agent team, including patent provenance.
- `CREDITS.md` and a filled copyright notice in the license header —
  practicing what the job preaches.

## For humans

Copy these folders somewhere your bot can reach — a synced Drive folder
works. Tell your bot: "Read `__init__/__init__.md` and start PLEX."
Say "stop PLEX" to deload it.

The language spec is `__init__/logic.md`. Read it first; every module's
header says what it may do. Kilo_CS's rule holds here: a module can't
widen its own permissions, and the closest rule wins.

## Layout

```
/__init__   the system (logic, plex modules)
/CORE       add-ons, loaded by core.md's loader
/JOBS       jobs and projects
/NOTES      shared logging and state
/MISSED     personal trash (moving a file here counts as move)
```

## Credit

Kilo_CS and the Kilo_CS language are the work of Tyler Starke
(profebral-beep), GPL-3.0. This fork keeps that licence and credit.
Card images are Kilo_CS's, same files. See CREDITS.md for the full
authorship record.
