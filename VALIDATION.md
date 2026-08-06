# Validation report

## Target

- Codex Desktop for Windows: `26.727.51351`
- Active native Codex home: `C:\Users\freeb\.codex`
- Package ID: `stella-materialism`
- Package format: V1 custom-pet package

V1 was selected for reliability on the installed Windows release. It uses the established 8×9 atlas and avoids the reported native-Windows V2 discovery issue.

## Atlas validation

- File: `run/stella-materialism/final/spritesheet.webp`
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

Frame extraction uses the Hatch Pet workflow's `stable-slots` mode. This was an intentional correction after the default component-fit extraction normalized every pose to the full cell height and suppressed the jump's vertical arc. The stable-slot review contains only the expected manual-review notices; the contact sheet and motion previews were subsequently inspected and accepted.

## Visual QA

- Identity: consistent short mint/teal layered hair, crown goggles, lime outlined eyes, freckles, reflective silver coat, black choker, dark clothing, mechanical gloves and utility boots
- Directional gait: right and left rows face correctly and alternate visibly
- Jump: clear low–high–low arc with no shadow, dust or detached effects
- Idle: subtle breath/blink loop
- Waiting, failure, active-work and review states: visually distinct
- Cropping, overlap, opaque backgrounds and guide marks: none observed
- Final visual QA: pass; repair rows: none

## Runtime package

Only `pet.json` and `spritesheet.webp` belong in the installed custom-pet directory. Development references, prompts, contact sheets and previews remain in this project.
