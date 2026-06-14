# Miliastra Wonderland L4D AI Director MVP

This folder contains a GIScript text-code prototype for an MVP implementation of a Left 4 Dead-style AI Director in Genshin Impact Miliastra Wonderland.

The repository itself is the GIScriptEditor compiler source. These files are intentionally kept in a separate example folder so they can be converted into UGC node graphs later without modifying the compiler.

## Important GIScript constraint

`ai_director_mvp.gis` only declares events from the GIScript VS Code extension `graph_events` list and only calls functions from the extension `builtin_functions` list. It does **not** declare custom helper functions or custom events, because those do not reliably convert into usable Miliastra Wonderland node graphs.

## MVP scope

The MVP focuses on the systems that create the strongest Left 4 Dead pacing effect with the fewest supported nodes:

1. **Survivor intensity**: stored in preset/custom values and updated from damage, combat, down/revive, and kill events.
2. **Adaptive dramatic pacing**: a four-state director loop: `0 = BUILD_UP`, `1 = SUSTAIN_PEAK`, `2 = PEAK_FADE`, `3 = RELAX`.
3. **Structured unpredictability**: mobs, specials, bosses, and loot use constrained random numbers plus designer-authored unit tags.
4. **Active area approximation**: instead of a full nav mesh, designers tag spawn-point entities by flow role, such as `director_spawn_behind`, `director_spawn_ahead`, `director_spawn_any`, and `director_boss`.
5. **Dramatic anticipation**: major events call built-in feedback nodes such as `print`, `PlayerPlaysOneShot2DSoundEffect`, and `ActivateScreenShake` before spawning threats.

## Files

- `ai_director_mvp.gis`: node-compatible GIScript event logic for conversion into Miliastra Wonderland node graphs.

## Designer setup assumptions

The script expects the UGC scene to provide designer-authored entities and data conventions:

- Timer IDs: `director_tick`, `director_mob`, `director_hunter`, `director_smoker`, `director_boomer`, and `director_boss`.
- Unit tags for spawn anchors: `director_spawn_behind`, `director_spawn_ahead`, `director_spawn_any`, `director_spawn_high`, `director_boss`, and optional loot tags.
- Prefab/config IDs are represented by placeholder `guid<prefab>` variables in the text code and should be replaced by real Miliastra assets before graph conversion.
- Preset/custom keys such as `director_state`, `p1_intensity`, `p2_intensity`, `team_flow`, and `last_boss_type` should be mapped to the project’s supported value-storage nodes.
