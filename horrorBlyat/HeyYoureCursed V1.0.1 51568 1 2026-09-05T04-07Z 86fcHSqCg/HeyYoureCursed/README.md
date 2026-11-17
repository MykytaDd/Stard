# Hey! You’re Cursed! — v1.0.0

A compact paranormal story mod for **Stardew Valley 1.6 + SMAPI 4.0+**.

A careless joke about ghosts leads to a cursed VHS on your doorstep, a ghost named **Sudoku** climbing into your life, a strange 18-stage puzzle bond, a Wizard who knows more than he admits, and a complete first supernatural case with multiple story callbacks.

## What v1.0.0 includes

- A persistent **Stardrop Saloon prologue** that waits until you actually attend.
- Compatibility-minded event deferral so another Saloon event can run first without Hey! You’re Cursed! chaining on top of it.
- A physical **morning parcel** outside the farmhouse. The VHS is only granted after you walk outside and inspect the package.
- The cursed VHS → TV → **Sudoku** arrival sequence.
- A real **Pencil** story gate; Pierre sells it for 100g.
- **18 Sudoku stages**, Daily Challenge, and Endless Practice after 18/18.
- Difficulty-based **Hints**: Easy 3, Normal 2, Hard 1.
- Daily Challenge keeps its normal reward and can add a small **gold performance bonus** for fast/no-hint clears.
- A separate **Trust 0–30** system with daily dialogue, gifts, activities, and max-Trust rescue.
- A seven-day **Wizard** milestone and placeable **Occult Cabinet**.
- Seal/unseal support which preserves Sudoku progress.
- A full **Spirit’s Eve** scene with three plan variants.
- A one-time 18/18 + Trust 30 capstone, **Channel 18**, and a seven-day epilogue.
- Keyboard, mouse, and controller support across the custom menus.
- UI sizing/fit safeguards for longer translated text.

## Compact compatibility philosophy

Sudoku is intentionally **not part of Stardew Valley’s vanilla friendship/social list**. She uses Hey! You’re Cursed!’s own Trust and Puzzle Bond systems instead. This keeps the social menu clean for large mod lists and avoids making future supernatural entities compete with ordinary villagers for vanilla friendship UI.

The mod also keeps Sudoku out of the vanilla calendar, introductions quest, Ginger Island visits, item-delivery quests, perfection friendship checks, and perfection slideshow.

## Languages

Included translations:

- English
- Vietnamese / Tiếng Việt
- French / Français
- Spanish / Español
- Simplified Chinese / 简体中文
- Japanese / 日本語
- Korean / 한국어
- Thai / ภาษาไทย

English is the final fallback language. Locale files share the same translation key set so switching languages cannot intentionally fall through to Vietnamese or another unrelated locale.

**Thai note:** Stardew Valley does not ship with Thai as a standard built-in language. `th.json` is included for custom-language setups using the `th` language code; the player’s language/font setup must provide Thai glyph support.

## Requirements

- Stardew Valley 1.6+
- SMAPI 4.0+

No Content Patcher or Generic Mod Config Menu dependency is required.

## Installation

1. Install SMAPI.
2. Extract the release ZIP into your Stardew Valley `Mods` folder.
3. The final path should be `Mods/HeyYoureCursed/manifest.json`.
4. Launch the game through SMAPI.

## Updating

Replace the old `HeyYoureCursed` folder with the new one. Do not merge old and new files together.

## Main story flow

1. Gus invites the farmer to the Stardrop Saloon around 18:00.
2. The farmer makes an unwise paranormal remark.
3. The next morning a brown-paper package waits by the farmhouse door.
4. Inspecting it grants the cursed VHS.
5. Using the VHS near the farmhouse TV begins Sudoku’s arrival.
6. Sudoku requires a real Pencil before the full relationship/gameplay loop activates.
7. Seven full days after Pencil activation, the Wizard delivers the Occult Cabinet.
8. Trust, 18-stage progression, Spirit’s Eve, the capstone, Channel 18, and the epilogue complete the first case.

## Debug/test commands

These are mainly for development and bug reports:

- `heyyourecursed_status`
- `heyyourecursed_test_help`
- `heyyourecursed_resetarrival`
- `heyyourecursed_test_prologue`
- `heyyourecursed_givevhs`
- `heyyourecursed_givepencil`
- `heyyourecursed_test_wizard`
- `heyyourecursed_givecabinet`
- `heyyourecursed_test_seal`
- `heyyourecursed_test_unseal`
- `heyyourecursed_test_solve`
- `heyyourecursed_test_profile`
- `heyyourecursed_test_trust`
- `heyyourecursed_test_stages`
- `heyyourecursed_test_endless`
- `heyyourecursed_test_spiriteve`
- `heyyourecursed_test_spiriteve_scene`
- `heyyourecursed_test_rescue`
- `heyyourecursed_test_capstone`
- `heyyourecursed_test_channel18`
- `heyyourecursed_test_epilogue`

## Building from source

For a normal Release build, run:

`Build_HeyYoureCursed.bat`

For a clean Nexus-ready ZIP, run:

`Build_Nexus_Release.bat`

The Nexus builder compiles `Release`, creates a clean `HeyYoureCursed` mod folder containing only runtime files, zips it, and writes a SHA256 checksum in `_release`.

## Version

**v1.0.0** is the first public complete release of the Sudoku case. Additional ghosts/cases are intentionally outside this release and can be added later without requiring players to complete them in a fixed linear chain.
