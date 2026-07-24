# Sync — Multicam Video Sync Tool

Automated multicam sync for video production. Matches multiple camera angles with audio class files using audio fingerprinting, then generates Premiere Pro XML timelines.

This repository only hosts the downloadable builds. The source lives in a
separate private repository.

## Download

👉 **[Download Latest Release](https://github.com/DanielGutierrezB/sync-releases/releases/latest)**

Each release lists what changed; there is no separate changelog here.

## Install

**macOS (Apple Silicon)**

1. Download `Sync-X.Y.Z-arm64.dmg`
2. Open the DMG and drag **Sync** to Applications
3. On first launch, right-click the app and choose *Open* — the build is not
   notarized, so a plain double-click is blocked by Gatekeeper

**Windows (x64)**

1. Download `Sync-Setup-X.Y.Z.exe`
2. Run the installer. SmartScreen will warn about an unknown publisher because
   the installer is not code-signed; choose *More info → Run anyway*

## Updates

The app checks this repository on startup and shows a banner when a newer
version exists. Because the builds are not code-signed, updates are **not**
installed in place: the banner opens the release in your browser, and you
reinstall over the previous version. Your settings and recent projects are
preserved.

## Features

- **Automatic multicam sync** — SD, BK, SR cameras matched to WAV class files via audio cross-correlation
- **Premiere Pro XML output** — Ready-to-import timeline projects
- **DaVinci Resolve export** — Optional FCPXML output
- **No-WAV mode** — Works without separate audio files
- **Whisper transcription** — Auto-transcribes classes for reference
- **Timeline viewer** — Verify sync visually before export

## Requirements

- macOS on Apple Silicon (arm64), or Windows x64
- Premiere Pro (or DaVinci Resolve) to open the generated projects

Not every release ships both platforms; check the assets on the release you are
downloading.
