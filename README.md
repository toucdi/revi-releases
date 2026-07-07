# Revi — Downloads

Private, on-device voice dictation for **macOS, Windows and Linux**.
App & pricing: **https://www.getrevi.app** — the easiest way to get Revi is
**[getrevi.app/download](https://www.getrevi.app/download)**, which detects
your OS automatically. This repo hosts the raw installer files and the
auto-update feeds; use the table below if you'd rather grab a file directly.

> The source code lives in a separate private repo — this one only hosts
> release binaries and update manifests.

## Download

| Platform | Recommended | Alternative formats |
|---|---|---|
| **macOS** (Apple Silicon) | [Revi-0.1.5.dmg](https://github.com/toucdi/revi-releases/releases/download/v0.1.5/Revi-0.1.5.dmg) | — |
| **Windows x64** | [Revi_0.1.4_x64-setup.exe](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_x64-setup.exe) | [.msi](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_x64_en-US.msi) · [portable .zip](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_x64_portable.zip) |
| **Windows ARM64** | [Revi_0.1.4_arm64-setup.exe](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_arm64-setup.exe) | [.msi](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_arm64_en-US.msi) · [portable .zip](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_arm64_portable.zip) |
| **Linux x64** | [Revi_0.1.4_amd64.AppImage](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_amd64.AppImage) | [.deb](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_amd64.deb) · [.rpm](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi-0.1.4-1.x86_64.rpm) |
| **Linux ARM64** | [Revi_0.1.4_aarch64.AppImage](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_aarch64.AppImage) | [.deb](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi_0.1.4_arm64.deb) · [.rpm](https://github.com/toucdi/revi-releases/releases/download/v0.1.4/Revi-0.1.4-1.aarch64.rpm) |

**Not sure which one you need?** Portable = unzip and run, no installer, no
admin rights, keeps its data next to the .exe (works from a USB stick).
Everyone else: use the installer (.exe/.msi/.dmg/.AppImage).

## Why the version numbers differ per platform

macOS (Swift, native) and Windows/Linux (Tauri) are built and released
independently, so they don't always share a version number. Each platform's
row above always points at its current stable release — that's normal, not
a mistake.

## Verifying downloads

- **Windows** binaries are Authenticode-signed (publisher: *Lumea di
  Georgiana Huides*) — right-click → Properties → Digital Signatures.
- **macOS** app is signed with a Developer ID and notarized by Apple — no
  Gatekeeper warning on first launch.

## All releases

Every version (including older ones and in-progress builds) is on the
[Releases page](https://github.com/toucdi/revi-releases/releases). Each
release lists every platform/architecture file for that version — if you're
on this page, you probably want the table above instead.

## Auto-update

The apps update themselves. macOS uses
[`appcast.xml`](https://www.getrevi.app/appcast.xml) (Sparkle); Windows/Linux
use [`latest.json`](https://github.com/toucdi/revi-releases/releases/latest/download/latest.json)
attached to the newest complete Windows+Linux release.
