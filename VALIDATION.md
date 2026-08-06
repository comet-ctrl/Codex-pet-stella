# Validation report

## Target

- Codex Desktop for Windows: `26.727.51351`
- Package ID: `stella-materialism`
- Package format: V1 custom-pet package

V1 was selected for reliability on the tested Windows release. It uses the established 8×9 atlas.

## Atlas validation

- File: `package/stella-materialism/spritesheet.webp`
- Encoding: WebP RGBA
- Dimensions: 1536×1872
- Grid: 8 columns × 9 rows
- Cell size: 192×208
- Required states: all 9 present
- Used frame counts: 6, 8, 8, 4, 5, 8, 6, 6, 6
- Unused cells: fully transparent
- Transparent-pixel RGB residue: 0 pixels
- Validator errors: 0
- Atlas validator warnings: 0

Frame extraction used the Hatch Pet workflow's `stable-slots` mode. This preserved the jump's vertical arc while keeping every animation aligned to the runtime grid.

## Visual QA

- Identity remains consistent across all animation rows.
- Directional gait faces correctly and alternates visibly.
- Jump follows a clear low–high–low arc with no shadow, dust, or detached effects.
- Idle uses a subtle breath/blink loop.
- Waiting, failure, active-work, and review states are visually distinct.
- No cropping, overlap, opaque backgrounds, or guide marks were observed.
- Final visual QA: pass; repair rows: none.

## Runtime package

Only `pet.json` and `spritesheet.webp` belong in the installed custom-pet directory. Development references, prompts, contact sheets, and previews are intentionally excluded from this repository.
