# Meow-Portal

An AI companion and illustrated desk for your Portal, with guided setup for Windows and Mac.

![Meow Desk on Portal](images/meow-desk.png)

## Release status

**In preparation. No public installer release is available yet.** Windows and Mac preview installers have been built, but physical-device update testing, Windows USB testing, distribution signing and the release review are still in progress. Downloads will appear under [Releases](https://github.com/dekayrekords-oss/Meow-Portal/releases) when ready.

This edition supports the tested Portal identified by Android as **omni**, running Android 10 with ARM64. Other Portal models are not yet verified. The planned desktop installers target Windows 10/11 x64 and macOS 13+ on Intel and Apple Silicon.

## How setup works

1. Open the Windows installer or the Mac application.
2. Select **Prepare connection**. The installer reuses installed Android SDK tools, or guides you through downloading verified tools from Google.
3. On Portal, open **Settings → Debug → ADB Enabled**, connect a USB data cable and approve the computer.
4. Select **Install Meow** or **Update / repair Meow** and leave the cable connected until verification finishes.

You must approve debugging on the Portal. The installer cannot enable it before authorization, and does not flash firmware. A compatible Windows USB driver may be required.

## Features

- Illustrated Desk with a companion, room objects and accessible navigation.
- **30 FPS avatar target** for fresh Portal setups. Saved settings are preserved; thermal and idle policies may reduce the actual frame rate.
- Guided compatibility, storage and app-integrity checks.
- In-place updates that do not deliberately clear existing app data.
- Local installer interface without telemetry or API-key collection.

AI provider accounts, credits and optional integrations are configured separately in Meow. Camera, voice and third-party integrations are still undergoing Portal validation. A separate ML Kit camera-optimization worker issue remains under investigation.

## User manual

[Download the offline user manual](https://github.com/dekayrekords-oss/Meow-Portal/raw/refs/heads/main/Meow-Portal-User-Manual.html), then open the downloaded HTML file in your browser. It covers installation, first setup, privacy, backups, updates and troubleshooting. It can also be printed to PDF from your browser.

Before a major update, export an encrypted backup from Meow and save it outside the Portal. Keep the password separately. The installer never needs your AI API keys.

## About this repository

This repository hosts public setup documentation and, when validated, downloadable release files. The Android application source and signing keys are private and are not included here. Automatic latest-version downloads will be enabled after a stable release is published and tested.

Meow is not affiliated with or endorsed by Meta. Third-party software and services remain subject to their respective terms. No open-source license for the Android application is granted by this repository.
