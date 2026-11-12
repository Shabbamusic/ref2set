# Ref2Set

Turn a reference song into an editable Ableton Live 12 Suite set (.als). The app is free and runs entirely on your Mac: your song is analysed locally, and the audio is deleted when each job finishes.

Website: https://analyze.shabbamusic.com/

## Download

Get the latest `Ref2Set-<version>.dmg` from [Releases](https://github.com/Shabbamusic/ref2set/releases). Each release lists its SHA-256 checksum. To verify your download:

```bash
shasum -a 256 ~/Downloads/Ref2Set-1.0.0.dmg
```

## What you need

- A Mac with Apple silicon (M1 or newer). Intel Macs are not supported.
- macOS 11 Big Sur or newer
- Ableton Live 12 Suite
- About 350 MB of disk space (116 MB download), plus about 1 MB per set

## Install

1. Open the DMG and drag **Ref2Set** into **Applications**.
2. Double-click Ref2Set. Ref2Set is not notarised by Apple yet, so macOS says it can't verify the app. Click **Done**.
3. Open **System Settings → Privacy & Security**, scroll to the line about Ref2Set, and click **Open Anyway**. Enter your password and confirm.
   You only do this once. On macOS 15 and newer, right-click → Open no longer skips it.
   Terminal alternative: `xattr -dr com.apple.quarantine /Applications/Ref2Set.app`
4. The first launch runs a one-time setup with a progress bar, which takes under a minute. Then drop a song into the console. A song takes about half its length to analyse.

## Closing and removing it

- Quit with ⌘Q, Dock → Quit, or the console's **Quit** button. Closing the console tab also stops it after a few seconds.
- Your sets are saved in `~/Library/Application Support/Ref2Set/sets`.
- To remove Ref2Set, delete the app and that folder.

© 2026 SHABBA Music
