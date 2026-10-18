# Qwnks' Console Experience: Refreshed

A lean, controller-first Minecraft experience built to feel like a console — with shaders,
atmosphere and quality-of-life, without the bloat.

**Minecraft 1.21.11** · Fabric & NeoForge · ~50 mods

---

## What is this?

**Qwnks' Console Experience: Refreshed** is a ground-up rebuild of the Qwnks' Console Experience modpack. It keeps the
console-inspired feel of the original while cutting the mod list roughly in half — removing
duplicate functionality, overlapping performance mods and unused libraries.

The result: the same vision, ~50 mods instead of ~85.

## Highlights

- **Controller-first** — full gamepad support via Controlify
- **Cinematic** — Iris shaders with Sodium, plus dynamic lighting
- **Atmosphere** — AmbientSounds, Sound Physics Remastered and footstep audio
- **Performance** — Sodium, Lithium, FerriteCore, ModernFix, ImmediatelyFast, EntityCulling, MoreCulling
- **Quality of life** — Inventory Profiles Next, Jade, AppleSkin, VeinMiner, FallingTree, Mouse Tweaks, Shulker Box Tooltip

## Branches

This repository holds both loader builds as separate branches. The mod list is functionally
identical across them.

| Branch | Loader | Mods |
| --- | --- | --- |
| [`main`](../../tree/main) | Fabric | 56 |
| [`neoforge`](../../tree/neoforge) | NeoForge | 50 |

A handful of mods differ between loaders (for example `continuity` → `fusion`, `PresenceFootsteps` →
`Tread Lightly`), and Essential is currently Fabric-only.

## Installation

1. Download the latest `.mrpack` from the [Releases](../../releases) page.
2. In **Prism Launcher**: `Add Instance` → `Import from zip` → select the `.mrpack`.

> The `.mrpack` is a small manifest — your launcher downloads the mods for you.

## Development

This pack is managed with [packwiz](https://packwiz.infra.link/), so every mod is described by a
small text file rather than a jar. To work on it:

```bash
git clone https://github.com/Qwnks/Qwnks-Console-Experience-Refreshed.git
cd Qwnks-Console-Experience-Refreshed

# add a mod (resolved from Modrinth)
packwiz modrinth add sodium

# update everything to the latest compatible versions
packwiz update --all

# export a distributable .mrpack
packwiz modrinth export
```

## Credits

- Pack curated by **Qwnks**
- All mods belong to their respective authors (see `mods/*.pw.toml` for sources)
- Licensed under the **BSD 3-Clause License** — see [LICENSE](LICENSE)
