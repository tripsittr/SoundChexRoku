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

**AGPL-3.0-or-later** — see [LICENSE](LICENSE). All SoundChex platforms share
this licence (AGPL §13).
