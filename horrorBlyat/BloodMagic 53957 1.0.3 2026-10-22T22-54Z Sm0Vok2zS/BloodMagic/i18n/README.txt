Blood Magic — SMAPI i18n (English base)

Copy default.json to a language file, such as es.json, fr.json, ja.json or pt-BR.json. Translate VALUES only. Preserve all {{token}} placeholders exactly (including capitalization).

Do not change Stardew control sequences (such as $h, $u, #$b#, ^^, [#], @, %item ... %%, or branch markers). If a translation alters protected codes, the game safely falls back to the original English for that entry. Slashes or double quotes in translated event speech are rejected.

assets/i18n_source_map.json maps older source text to translation keys; do not translate or edit that file.

The separate [CP] Blood Magic content pack is NOT included. Its translations require the pack source and its own i18n files. This patch covers the main C# mod only.

A game restart is recommended after changing item, NPC, event, or mail translations. No translated language files are included yet.
