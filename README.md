# Stella — Codex Desktop Pet

An unofficial, fan-made custom pet for Codex Desktop inspired by Stella from Studio Wrong's *Stella's Materialism*.

![Stella pet preview](preview.png)

## Install

### Option 1: PowerShell

1. Download this repository with **Code → Download ZIP**, then extract it. You can also clone it with Git:

   ```powershell
   git clone https://github.com/comet-ctrl/Codex-pet-stella.git
   cd Codex-pet-stella
   ```

2. Copy the pet package into your Codex pets directory:

   ```powershell
   $destination = Join-Path $env:USERPROFILE ".codex\pets\stella-materialism"
   New-Item -ItemType Directory -Force -Path $destination
   Copy-Item ".\package\stella-materialism\*" $destination -Force
   ```

3. In Codex Desktop, open **Settings → Appearance → Pets**.
4. Refresh custom pets if Stella is not listed, then select **Stella**.

### Option 2: Manual installation

Copy the entire [`package/stella-materialism`](package/stella-materialism) folder to:

```text
%USERPROFILE%\.codex\pets\stella-materialism
```

The installed folder must contain both files directly:

```text
stella-materialism/
├── pet.json
└── spritesheet.webp
```

Restart Codex Desktop or refresh custom pets if the pet does not appear immediately.

## Uninstall

Delete `%USERPROFILE%\.codex\pets\stella-materialism`, then restart Codex Desktop.

## Package details

The pet uses a Codex V2 custom-pet atlas: 1536×2288 pixels, arranged as an 8×11 grid of 192×208 cells. The final two rows provide 16 clockwise look directions. The repository contains only the runtime package and concise documentation; generation prompts, intermediate frames, QA media, and downloaded references are intentionally excluded.

## About the artwork

This project contains newly generated fan art and does not redistribute frames from Studio Wrong's videos. It is not affiliated with, endorsed by, or sponsored by Studio Wrong.

See [CREDITS.md](CREDITS.md) for source links and the fan-project notice. Technical validation notes are available in [VALIDATION.md](VALIDATION.md).
