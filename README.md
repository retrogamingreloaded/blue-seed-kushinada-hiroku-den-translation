# Blue Seed: Kushinada Hirokuden — English Translation

English fan translation and preservation project for **Blue Seed: Kushinada Hirokuden** on Sega Saturn.

*** STILL IN BETA - EXPECT SOME ISSUES IN TRANSLATION ***

Testing and translation review of the current build are in progress. We are looking for volunteers to test it and report any translation or display issues.

## Project status

The latest candidate updates 38 text entries and fixes a stray glyph before the bridge dialogue. It standardizes card names and card-gain notices, fixes a dialogue indentation and punctuation, and consistently uses Ushitora for the traditional northeast direction.

- Automated checks verified rebuilt glyphs, window bounds, interactive choices and disc readback. Only 15 disc files changed from v0.1.11-beta. The map-label fixes from that version are unchanged.
- The full xdelta patch and macOS application script reproduce the target byte for byte from the verified original Japanese Track 01. Windows execution has not been tested.
- Translation review and in-game playtesting are ongoing. Automated checks do not replace a visual check in-game. The reading of constable 大田原 (provisionally Otawara) remains uncertain.

A ROM-free test patch is available: **[English Test Patch v0.1.12-beta](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.12-beta)**. The preceding [v0.1.11-beta](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.11-beta) remains available separately.

This remains a pre-release build while full-game proofreading and visual QA continue. See the [changelog](CHANGELOG.md) for earlier updates.

## Playtesters wanted

We are looking for volunteers to playtest the English beta while our review continues. If you spot a translation error, clipped or overlapping text, unusual glyphs, broken line breaks, or misaligned dialogue, choices, or menus, please [open a GitHub issue](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/issues/new).

Please include the patch version, chapter or location, the text or screen affected, your emulator/core and version, and steps to reproduce the problem. A screenshot is helpful when available. Do not upload ROMs, BIOS files, or save data.

## Save compatibility

Sega Saturn backup-memory saves can be retained between translation builds when the same RetroArch content filename and core are used. Always back up save files before replacing a build.

Save states are more fragile and may be incompatible between different builds or emulator/core versions. In-game saves are strongly recommended for long-term progress.

## Download and patching

Download the ZIP package from the [v0.1.12-beta release page](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.12-beta). It contains the xdelta patch, checksum manifest, English CUE file, and patching scripts/instructions for macOS, Linux/Steam Deck, and Windows. The xdelta patch has been decoded against the required Japanese source and reproduces the published target checksum exactly. This full patch requires the Japanese source, not a previous English BIN. It remains a work-in-progress test candidate, not a final-quality release.

The patch requires a legally obtained Japanese Track 01 with this SHA-256 checksum:

`1a9ce56a4746320f326fcc1269442ecf1917893d0e9feaf75030e98012d88b0f`

### Windows patching — untested

**This Windows procedure has not been tested: the maintainer does not have a Windows PC. Windows testers are welcome to report whether it works or any problems encountered.**

1. Download and extract `blue-seed-english-v0.1.12-beta.zip` from the release page. Keep the extracted files together; do not run the script from inside the ZIP.
2. Download an appropriate Windows **xdelta3** binary from the [official xdelta releases](https://github.com/jmacd/xdelta/releases). Extract it and place the executable beside `apply-patch.ps1`, naming it `xdelta3.exe` if necessary. Alternatively, make `xdelta3.exe` available on your PATH.
3. Keep your original Japanese Track 01 and all original audio tracks 02–29 together, with their original filenames. Use the Japanese source whose checksum is shown above, not a previous English build. Back up your saves before updating.
4. Open PowerShell in the extracted patch folder, or change to it with the first command below. Replace both example paths with your own paths, keeping the quotes:

```powershell
cd "C:\Games\blue-seed-english-v0.1.12-beta"
powershell.exe -NoProfile -ExecutionPolicy Bypass -File .\apply-patch.ps1 "D:\Games\Blue Seed - Kushinada Hirokuden (Japan) (Track 01).bin"
```

The execution-policy option applies only to that PowerShell process; it does not permanently change your Windows settings. Only run the script from the trusted release package.

The script is designed to verify the source and reconstructed output checksums and require all original audio tracks. It creates `Blue Seed - Complete English (Track 01).bin` and `Blue Seed - Complete English.cue` beside the Japanese source. It refuses to overwrite an existing English BIN, CUE or partial output; use a separate folder containing your original Japanese tracks if an older English build is already present. Do not delete your saves.

After a successful patch, open **`Blue Seed - Complete English.cue`** in your Saturn emulator, not the BIN or xdelta file. Keep all original audio tracks beside it.

No ROM, disc image, BIOS, or unauthorized copyrighted game asset will be distributed by this repository.
