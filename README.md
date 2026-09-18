# SoundChex for Roku

The SoundChex client for **Roku** — its own repo because Roku is a closed
platform with a proprietary language (**BrightScript**) and UI framework
(**SceneGraph**) that shares no code with any other target.

It talks to the SoundChex server's JSON API (`/api/v1/*`) for browse, streaming,
progress and search, and plays through Roku's native video pipeline.

## Why standalone

BrightScript/SceneGraph is unique to Roku — no shared runtime with the Android,
Swift, or web clients. A Roku channel is built with Roku's SDK and published (or
sideloaded in developer mode) as its own artifact.

## Planned stack

- **BrightScript + SceneGraph** (`.xml` scene graph + `.brs` logic).
- Roku's `roVideoPlayer` for playback against the token-authed stream endpoint.
- Grid/details screens driven by the same catalogue API.

## Status

Scaffold only — see [Documentation & Planning/Status.md](Documentation%20&%20Planning/Status.md)
and [Roadmap.md](Documentation%20&%20Planning/Roadmap.md). No channel code yet.

## Licence

**Dual-licensed** — **AGPL-3.0-or-later** by default (see [LICENSE](LICENSE)), or
a **commercial licence** for those who can't/won't comply with the AGPL. Full
terms, the contributor agreement, and the commercial option live in the main
repo: [LICENSING.md](https://github.com/tripsittr/SoundChex/blob/main/LICENSING.md)
(contact `licensing@soundchex.app`). AGPL §13: a modified, network-hosted build
must offer its users the corresponding source.