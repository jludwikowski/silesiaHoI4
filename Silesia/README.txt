# Silesia (SIL) HOI4 Focus Tree

## Included
- `common/national_focus/silesia.txt` — full focus tree
- `common/ideas/silesia.txt` — national spirits
- `common/characters/SIL.txt` — four ideological leaders
- `common/country_leader/SIL_traits.txt` — custom leader traits
- `common/ai_strategy_plans/SIL_ai.txt` — AI focus plans
- `localisation/english/SIL_l_english.yml` — English localization

## State ID assumption
This package assumes the standard vanilla state IDs:
- 66 = Lower Silesia
- 67 = Upper Silesia
- 72 = Zaolzie
- 69 = Sudetenland

## Important compatibility note
This is intended as a drop-in content layer for an existing SIL country tag. It deliberately does NOT overwrite:
- `common/country_tags/`
- `history/countries/`
- `history/states/`
- flags
- map files

This minimizes conflicts with the existing Silesia implementation.

## Ideology
The four branches use vanilla ideology groups:
- monarchy: non-aligned / neutrality
- fascist: fascism
- communist: communism
- democratic: democratic

No custom ideology definitions are required.

## Testing
Start a NEW GAME after installing. `on_startup` does not retroactively initialize an already-created save.

Use `-debug` and check `error.log` if the tree fails to load. The most likely compatibility issue is changed state IDs or an existing SIL focus tree using one of the same IDs.
