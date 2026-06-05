# bg2ee-zx-items

Proper-ish BG2EE ToB/WK late-game custom items for a personal SoA/ToB campaign.

## Scope

Small BG2EE item pack for a specific late-game party.

Not a quest mod. Not a public balance package. Items are currently installed as resources and added manually by console.

## Supported game

BG2EE only.

EET is not targeted or tested.

## Installation

Install with WeiDU.

The installer copies prepared item/spell resources and applies required table rows.

Unidentified item names/descriptions are intentionally left generic. Only identified names/descriptions are replaced.

## Console injection

```baf
C:CreateItem("ZXAMUL1")
C:CreateItem("ZXAMUL2")
C:CreateItem("ZXCHAN1")
C:CreateItem("ZXHELM1")
C:CreateItem("ZXPLAT1")
C:CreateItem("ZXSW1H1")
C:CreateItem("ZXSW1H2")
```

## Intended timing

- `ZXAMUL2` — Imoen; after Spellhold / soul-restoration arc.
- `ZXAMUL1` — CHARNAME; after Hell, at the start of ToB.
- Other items — mid-to-late ToB, especially around Watcher's Keep progression.

These are late-game consolidation/capstone items, not early-game power items.

## Items

### `ZXAMUL1` — Amulet of the Tempered Will

CHARNAME-oriented fighter/mage amulet.

Post-Hell / start-of-ToB personal reward. Improves combat accuracy, saves, MR, casting speed, wizard spell slots, poison immunity, level-drain immunity, and grants 1/day instant Death Ward.

### `ZXAMUL2` — Amulet of the Returned Soul

Imoen-only amulet.

Post-Spellhold / soul-restoration reward. Improves Dexterity, AC, saves, MR, casting speed, wizard spell slots, Vocalize, and grants 1/day instant Negative Plane Protection + Death Ward.

### `ZXCHAN1` — War Wizard's Mithral Chain

Fighter/mage-style mithral chain.

An updated, reforged, stabilized drow-chain concept: arcane casting allowed, casting speed reduced by 2, plus THAC0, saves, MR, and movement-effect protections.

Not a Robe of Vecna replacement. Vecna remains the superior pure-caster item.

Added to `ITEMEXCL.2DA`.

### `ZXHELM1` — Helm of the Watchful Mind

Practical command helm.

Provides critical-hit protection, AC, THAC0, saves, MR, infravision, Vocalize, blindness immunity, and deafness immunity.

### `ZXPLAT1` — Battle-Priest's Full Plate +3

Divine-caster-oriented full plate.

Strong armor with saves, casting-speed help, and 1/day emergency combat/casting burst.

Added to `ITEMEXCL.2DA`.

### `ZXSW1H1` — Blade of Finality +4

Late-game katana.

Critical-focused main weapon with stun, critical-hit slay chance, and a limited-use high-enchantment / high-accuracy killing window.

Uses `ZXSW1H1.SPL` for the critical-hit death effect.

### `ZXSW1H2` — Faithful Companion +3

Late-game wakizashi/off-hand blade.

Adds an extra attack per round, off-hand THAC0, AC, slashing AC, and saves.

## Installer notes

The installer mainly:
- copies `.ITM` and `.SPL` resources;
- assigns identified item names and descriptions;
- appends `ITEMEXCL.2DA` rows for the armors;
- appends an `ITEM_USE.2DA` row for Imoen's amulet.

## Status

Private/personal beta.
