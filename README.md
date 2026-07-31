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

**v0.9.2** — pre-release. All nine attachment slots modeled. See Open Questions for what is still missing.

## Changelog

### v0.9.2

**Additions**

- Weapon cards. Every automatic weapon, stock, with its shots-to-kill band by range, hipfire and aimed reach, dispersion ceilings, and a named counter for its worst stat.
- Stat families split by range. `+mACC` scales up with range, `+mSPD` scales down, `+HIP` and `+ADS` stop mattering past the hipfire band.
- Named counters table, keyed to thresholds you can read straight off a card.

**Removals**

- Untracked Mechanics
- Class-restricted attachments
- Cross-slot interactions

**Editorial**

- Trimmed down several sections for an attempt at brevity.
- Slot sections reordered to match the allocation steps.
- 79 em-dashes removed in favor of proper grammar.

### v0.9.1

**Corrections**

- Ribbed Stubby no longer incorrectly lists `+mSPD`.
- `−SEEN` redefined: the laser projects a beam roughly 5m into world space, revealing position rather than presence. Red and Violet are positionally quiet, not invisible — the 20–30 point tier is not disqualified for stealth builds.
- Rule 2 no longer claims high-rung grips are unaffordable for mobile players. Both drawbacks have counters.
- Rule 4 narrowed: mounting is the only thing that improves on standing still, not the only purchasable spread reduction.
- Fire-mode attachments marked weapon-specific rather than competing choices.

**Additions**

- Burst Training (15, ergonomics) and the `BURST` tag.
- `VARZOOM` split into `ZTOGGLE` and `ZCYCLE`. The two-magnification optics
  and the multi-magnification ones are priced differently and now read that
  way in the table.
- `+mSPD` and `+PEN` added to the component costs in Rule 1.
- sym.gg and the ADS Spread Simulator linked where they are useful, not just
  in Sources.

**Editorial**

- Removed overstating language throughout.
- Colour-coded callouts by audience: blue is addressed to an assistant, amber
  to you, red is a warning, green is a finding.

### v0.9

Initial release.

## Corrections

Open an issue. Tooltip transcriptions and per-weapon costs are especially welcome — the magazine slot and the headshot/subsonic ammo are the two places costs genuinely vary per weapon.

## License

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) — share and adapt with credit, non-commercial, derivatives under the same license.

Compiled and written by **AntiPhysicsGames**, 2026.

Battlefield 6 is a trademark of Electronic Arts Inc. Unofficial fan reference, not affiliated with EA or DICE.
