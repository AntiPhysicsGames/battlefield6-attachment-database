# BF6 Attachment Database

A reference for Battlefield 6 attachments: what they do, what they cost, and how they change a weapon's stats. Every value is read straight off the in-game screens.

**Read it here:** https://antiphysicsgames.github.io/battlefield6-attachment-database/

---

## What this is

Most BF6 attachment databases copy the same stat bars, and those bars leave out the mechanics that actually decide a build. This one is built one gun at a time from the in-game build menu, and covers:

- **Every attachment** with its cost, type, tags and stat changes. Attachments that do the same thing under different names share an entry.
- **A tag vocabulary** for every effect and drawback, including the ones the stat bars don't show: recoil buildup, moving ADS accuracy, laser visibility, spotting ranges.
- **Point costs for every tag.** Each attachment's cost is checked against the sum of its tags.
- **A build menu.** Pick an attachment per slot and watch the stats change as you hover. Builds can be shared by link and pinned for comparison.
- **The four in-game bars**, with the formula behind each one.
- **Open questions**, listed on the site rather than guessed at.

If a value hasn't been read in game, it's left blank.

## Status

**v0.9.4**: pre-release. The M433 is fully recorded; more weapons are being added one at a time.

## Changelog

### v0.9.4

**Rebuild**

- Rebuilt from a single long document into a searchable encyclopedia with a sidebar, attachment pages, weapon pages and a reference section.
- All weapon and attachment data re-read from the game. v0.9.3 values that haven't been re-checked are labelled as such.

**Additions**

- Build menu: live stat preview, green and red changes, share links, pin to compare, sorting and filtering inside each slot, keyboard controls.
- Optics recorded by name, with the optic accessories each one enables.
- Right Accessory split from Top Accessory.
- Tags: `LINEAR`, `BLIND`, `AUTO`, `THERMAL`, `VARIABLE`, `MAG`.
- Point cost on every tag, with a cost check on every attachment.
- Mobility worked out in steps: each ADS step is 4, each draw step 2, each ADS move speed tier 2, each moving ADS accuracy tier 4. It matches 57 of 59 weapons exactly.
- What each tag does on the stats panel, with ranges that narrow as more weapons are added.
- Search by tag combination, e.g. `+ADS -mACC`.
- Season accent colours, light and dark themes, phone and 4K modes.

**Corrections**

- `hREC` replaced by `LINEAR`: the Linear Compensator trades horizontal recoil for vertical.
- Hipfire steps move along the hipfire table (+7, +7, +8 on the M433), not a flat amount.
- Barrel velocity changes are percentage-based on the M433 (×1.25 Extended, ×0.80 Short).

**Removals**

- Weapon cards, shots-to-kill bands and named counters.
- Barrel, ammo and optic archetypes, replaced by real attachment names.
- The pricing formula, replaced by per-tag costs.
- The error log.
- The "For the assistant" section.

**Editorial**

- Descriptions rewritten in one short style. Lines that only say what an attachment doesn't do were dropped.

### v0.9.3

**Corrections**

- Recoil ladder is linear: `+REC4` and `+REC5` cost corrected.
- `+mSPD` cost corrected.
- Lights grant `+HIP-RBLD`, hipfire spread recovery, not hipfire accuracy.
- Laser/Light Combo Red and Green added. Removed from the error log.
- Draw speed updated.
- `−SEEN` renamed `VISIBLE`. It names a property, not a drawback.

**Additions**

- `+HIP-RBLD` tag.
- Numbered sections and a table of contents.
- Jump links throughout. Tags, attachments, archetypes, slots and rules.
- Hipfire drawn as a band on each card, showing the cone widening as you fire.

**Removals**

- The range-coverage system
- The optic tags: `ZTOGGLE`, `ZCYCLE`, `THERM`, `MAGNIFIER`, `PIGGYBACK`
- How to build a loadout

**Editorial**

- Optics collapsed to six classes.
- Shortened Tag Legend.
- Weapon cards reworked: Squirreliness, Climb and Spread, each ranked against the roster.

### v0.9.2

**Additions**

- Weapon cards. Every automatic weapon, stock, with its shots-to-kill band by range, hipfire and aimed reach, dispersion ceilings, and a named counter for its worst stat.
- Stat families split by range.
- Named counters table.

**Removals**

- Untracked Mechanics
- Class-restricted attachments
- Cross-slot interactions

**Editorial**

- Trimmed down several sections.
- Slot sections reordered to match the allocation steps.

### v0.9.1

**Corrections**

- Ribbed Stubby no longer incorrectly lists `+mSPD`.
- `−SEEN` redefined as a beam revealing position.
- Rules 2 and 4 narrowed.
- Fire-mode attachments marked weapon-specific.

**Additions**

- Burst Training and the `BURST` tag.
- `VARZOOM` split into `ZTOGGLE` and `ZCYCLE`.
- sym.gg and the ADS Spread Simulator linked where useful.

**Editorial**

- Removed overstating language.
- Colour-coded callouts by audience.

### v0.9

Initial release.

## Corrections

Open an issue. In-game readings are especially welcome: a weapon's stats panel, or what an attachment changes on it.

## License

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/): share and adapt with credit, non-commercial, derivatives under the same license.

Compiled and written by **AntiPhysicsGames**, 2026. Support the project on [Ko-fi](https://ko-fi.com/R8Q4245SX2).

Battlefield 6 is a trademark of Electronic Arts Inc. Unofficial fan reference, not affiliated with EA or DICE.
