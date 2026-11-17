# Credits and AI usage evidence

Updated 2026-11-18 for Web 0.1.38. Creator: **BigTin**, individual entrant; creative direction, selection and release decisions. The AI/art contributions remain those documented for 0.1.37; 0.1.38 changes touch-hint wording only. This is an evidence inventory, not a claim that every asset in the shipping build has been audited. Retain the source licenses with distributed materials where applicable.

## Verified in this repository

| Component | Source / role | Evidence |
| --- | --- | --- |
| Space models | Kenney Space Kit 1.0; bundled license states CC0 | `StarlightRepair/Assets/ArtCandidates/KenneySpaceKit/License.txt`; source URLs and archive SHA256 in `Docs/ArtSources.txt` |
| Space base models | Kay Lousberg, KayKit Space Base Bits 1.0; bundled license states CC0 | `StarlightRepair/Assets/ArtCandidates/KayKitSpaceBase/LICENSE.txt`; source commit/archive information in `Docs/ArtSources.txt` |
| Pirate ship | Kenney Pirate Kit 2.1; bundled license states CC0 | `StarlightRepair/Assets/ArtCandidates/KenneyPirateKit/License.txt`; source archive in `ArtSources/KenneyPirateKit/` |
| Font | Nanum Gothic; bundled SIL Open Font License 1.1 | `StarlightRepair/Assets/_Project/Fonts/OFL.txt` |
| Main menu illustration | Built-in OpenAI image generation, documented generation date 2026-11-05 | `Tools/Art/MainMenuPrompt.txt`; `Docs/ArtSources.txt`; output at `Assets/_Project/PlanetVoyage/UI/Resources/MainMenu/Home.png` |
| Menu/action icons | Project SVG and generated icon tooling | `Tools/Art/MainMenuIcons.svg`, `FlightActions.svg`, `FlightDefense.svg`, `FlightHudIcons.cjs` |
| Sector skies | Project rendering/generation code | `Tools/Art/GenerateSectorSkies.cjs`, `LowerSectorSkies.cjs` |
| Music and sound effects | Procedural synthesis and arrangement in project code; two 45-second exploration loops and action cues | `Tools/Art/FlightSound.py`, generated assets in `Assets/_Project/PlanetVoyage/Audio/Resources/FlightSound/` |
| Development assistance | OpenAI Codex assisted code review, implementation, localization, and validation during this preparation session | Current development chat and resulting repository changes; preserve the relevant session/export if needed |
| Opening and ending cinematics (2026-11-15) | Built-in OpenAI image generation; project-authored camera, pixel composition, animation and type; HyperFrames/GSAP rendering; existing project music and sound effects | `Cinematics/Starlight-Cinematics-v02/ASSETS.md` and `Cinematics/HomeAtLast-Ending-v01/ASSETS.md`; original generation IDs retained; clean 10-second opening trimmed/faded with FFmpeg, 15-second reopening and 15-second Home at Last true ending; no AI voiceover |
| Disaster and shield sound effects (0.1.36) | Original deterministic procedural synthesis, using harmonics, filtered noise and envelopes | `hazards()` in `Tools/Art/FlightSound.py`; SolarAlert, PirateAlert, SolarWindLoop, ShieldReflect and ShieldWave; 25-asset signal and maximum-volume mix checks in `flight-audio-signals-0.1.36.json` |
| Healing activities (0.1.37) | Reuses the existing CC0 R01–R03 robot, S04 courier, P08 cargo prefabs and KayKit wind turbine models; no new external model or AI image assets | `Assets/_Project/Editor/HealingAssetBuilder.cs`; resource catalog `Assets/_Project/PlanetVoyage/Resources/HealingAssets.asset`. Wake trails, water jets, beacons, coin effects and drifting lights are drawn in project code. |

Paths beginning with `Assets/` above are relative to the `StarlightRepair` Unity project. Other paths are relative to the repository root.

## Honest AI-use statement draft

> I used OpenAI tools as part of an iterative development workflow. The main menu illustration was generated from a project-specific visual brief, with the prompt retained in the repository. Codex assisted with programming, debugging, localization, and review. The game combines that work with credited asset packs and project-authored procedural graphics and audio tools. Creative direction, selection, iteration, and final release decisions remain with the creator.

The final sentence is for the creator to review before submitting. Add other tools only when actual use and the relevant evidence are available. Do not label the procedural audio as ElevenLabs output, the CC0 models as Meshy output, or all art as AI-generated. No evidence for those claims was established by this review.

## Before final submission

- Creator display name and individual status confirmed as BigTin on 2026-11-18.
- Check that the final build's dependent assets match this inventory, including packages, plugins, shaders, and any newer assets added after this review.
- Preserve image-generation provenance and review the applicable tool terms for the actual account used at creation.
- Keep third-party reference screenshots in development documentation separate from the game and promotional exports. `Docs/ArtReview/SpaceReferences/` contains visual references, which are not established as distributable game art by this inventory.
- Confirm that gameplay footage, music, logos, and screenshots in the final submission are from this game or have the required permissions.

The official competition requires accurate AI disclosures and appropriate rights for submitted content. Tool-specific awards require evidence of the relevant tool's use. [Chroma Awards official rules](https://chromaawards.com/terms)
