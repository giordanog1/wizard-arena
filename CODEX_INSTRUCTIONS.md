# CODEX INSTRUCTIONS — WIZARD ARENA

You are maintaining WIZARD ARENA.

Before changing code, read `WIZARD_ARENA_BIBLE.md`.

## Hard rules
- Keep the game as a single-file HTML build unless the user explicitly asks for a multi-file refactor.
- Preserve the locked visual/gameplay identity.
- Keep gameplay canvas at native 390x844.
- Keep wizards as plain elemental circular balls with HP centered inside each ball.
- Keep weapons/staffs hovering or orbiting around the balls; weapons never cover HP.
- Never rename or recolor AQUARIUS, ZEPHYR, IGNIS, or TERRA.
- Preserve elemental advantages: Water > Fire, Fire > Earth, Earth > Air, Air > Water at 2x; reverse is 0.6x.
- Keep damage counters, live stats, abilities, MVP screen, battle recorder, and video download flow.
- Do not redesign core systems unless explicitly requested.
- Use project assets from `/assets` when adding new visual content.
- Every update must produce a working `index.html`.
- Test JavaScript syntax before finishing.
- Do not claim a file exists unless it was actually created.

## Preferred change process
1. Identify the smallest layer to change.
2. Preserve all locked systems.
3. Update `index.html`.
4. Run a JS syntax check by extracting the script section or opening it in a browser/dev server.
5. Summarize the change in a short changelog.

## Common tasks
- Add a new episode modifier.
- Add a new ability while preserving existing abilities.
- Swap or add Battle Master announcer expressions.
- Add new hover weapons, hats, or environmental hazards.
- Improve effects, sounds, stats, or recorder/export quality.

## Current Battle Master assets
- `assets/battle-master/masterwizard_spritesheet.png` contains four expressions:
  - top-left: neutral
  - top-right: happy
  - bottom-left: angry
  - bottom-right: laughing
- Pre-sliced versions are also included where available.

## Current staff assets
- `assets/staffs/ignis_fire_staff.png`
- `assets/staffs/aquarius_water_staff.png`
- `assets/staffs/terra_earth_staff.png`
- `assets/staffs/zephyr_air_staff.png`
