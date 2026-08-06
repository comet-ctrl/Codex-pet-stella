# Validation report

## Target

- Codex Desktop for Windows: `26.727.51351`
- Package ID: `stella-materialism`
- Package format: V2 custom-pet package

## Atlas validation

- File: `package/stella-materialism/spritesheet.webp`
- Encoding: WebP RGBA
- Dimensions: 1536×2288
- Grid: 8 columns × 11 rows
- Cell size: 192×208
- Standard animation rows: 9
- Look-direction cells: 16
- Sprite version: 2
- Unused cells: fully transparent
- Transparent-pixel RGB residue: 0 pixels
- Validator errors: 0
- Atlas validator warnings: 0

## Visual QA

- Identity remains consistent across all animation rows.
- Directional gait faces correctly and alternates visibly.
- Jump follows a clear low–high–low arc with no shadow, dust, or detached effects.
- Idle uses a subtle breath/blink loop.
- Waiting, failure, active-work, and review states are visually distinct.
- The 16-direction loop passes visual review; a few intermediate diagonal up/down cues are intentionally subtle.
- No cropping, overlap, opaque backgrounds, or guide marks were observed.
- Final visual QA: pass; repair rows: none.

## Runtime package

Only `pet.json` and `spritesheet.webp` belong in the installed custom-pet directory. Development references, prompts, contact sheets, and previews are intentionally excluded from this repository.
