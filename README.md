# BF6 Attachment Database

A reverse-engineered reference for Battlefield 6 attachments — what they actually do, what they cost, and the pricing formula that governs all of it.

**Read it here:** https://antiphysicsgames.github.io/battlefield6-attachment-database/

---

## What this is

Every public BF6 attachment database copies the same stat bars, and those stat bars are missing the mechanics that actually decide a build. This document is built from in-game tooltips, cross-referenced against datamined tables, and covers:

- **A tag vocabulary** for every effect and drawback, including the ones no source tracks — recoil buildup, ADS accuracy while moving, laser visibility, spotting ranges
- **Six tiered stat ladders** — ADS, draw, recoil, hipfire and more move in discrete rungs, not continuous values
- **A pricing formula** that predicts any attachment's cost from its effects, verified against every muzzle, grip, barrel archetype and ammo type
- **Archetype models** collapsing 163 barrel names into 11 archetypes and the ammo slot into 15
- **An error log** of what the public sources get wrong, including three attachments that do not exist in the game

## Using it with an LLM

The document is a model, not a dataset — it explains how attachments behave and how they are priced, and leaves the two genuinely weapon-specific figures to be read in game. That split is what makes it useful to hand to a model.

Paste this with your weapon name:

```
Reference: https://antiphysicsgames.github.io/battlefield6-attachment-database/

Read the "For the assistant" section at the end of that page before you start.

Building a loadout for the [WEAPON].
```

Point at the section explicitly — it sits at the end of a long page and models frequently stop before reaching it. Everything else in the document they find on their own.

## Status

**v0.9** — pre-release. All nine attachment slots modeled. See Open Questions for what is still missing.

## Corrections

Open an issue. Tooltip transcriptions and per-weapon costs are especially welcome — the magazine slot and the headshot/subsonic ammo are the two places costs genuinely vary per weapon.

## License

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) — share and adapt with credit, non-commercial, derivatives under the same license.

Compiled and written by **AntiPhysicsGames**, 2026.

Battlefield 6 is a trademark of Electronic Arts Inc. Unofficial fan reference, not affiliated with EA or DICE.
