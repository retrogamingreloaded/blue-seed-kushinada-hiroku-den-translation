# Blue Seed: Kushinada Hirokuden — English Translation

English fan translation and preservation project for **Blue Seed: Kushinada Hirokuden** on Sega Saturn.

*** STILL IN BETA - EXPECT SOME ISSUES ***

Testing and translation review of the current build are in progress. We are looking for volunteers to test it and report any translation or display issues.

## Project status

The latest candidate includes 5,157 ordinary text entries and ten embedded text tails, with 2,868 documented ordinary correction IDs and two separately maintained embedded-text corrections.

- Review records now cover all 4,384 model-unflagged passages and 783 adjudicated passages. This completes that review-record backlog, not final semantic approval. Constable 大田原, provisionally Otawara (03188), remains an uncertain reading.
- Map-label fixes restore clipped final letters, closing parentheses and arrow clearance. All 385 instances (35 labels across 11 maps) pass raster/bounds checks. Large Japanese background lettering is not translated by this change.
- All 50 build stages pass, including repeatable MES/EXE rebuilding, 104 injected-file readbacks and glyph/window checks covering 3,021 proof IDs at 3,467 rebuilt locations. All 79 detected interactive menus / 178 locations retain selection commands and row geometry. The 97 tool unit tests pass.
- The full xdelta patch and macOS application script reproduce the target byte for byte from the verified original Japanese Track 01. Windows execution has not been tested for this update.
- This candidate was deployed to Steam Deck on October 25, 2026 with its installed checksum verified. This exact image has not received a new emulator startup or full-game validation; older startup checks concern earlier candidates.
- Full-game playtesting, dialogue branches, visual review and save/reload checks remain to be completed. Automated checks and complete review records do not certify every translation or screen.

A ROM-free test patch is available: **[English Test Patch v0.1.11-beta](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.11-beta)**. The preceding [v0.1.10-beta](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.10-beta) remains available separately.

This remains a pre-release build while full-game proofreading and visual QA continue. See the [changelog](CHANGELOG.md) for earlier updates.

## Playtesters wanted

We are looking for volunteers to playtest the English beta while our review continues. If you spot a translation error, clipped or overlapping text, unusual glyphs, broken line breaks, or misaligned dialogue, choices, or menus, please [open a GitHub issue](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/issues/new).

Please include the patch version, chapter or location, the text or screen affected, your emulator/core and version, and steps to reproduce the problem. A screenshot is helpful when available. Do not upload ROMs, BIOS files, or save data.

## Save compatibility

Sega Saturn backup-memory saves can be retained between translation builds when the same RetroArch content filename and core are used. Always back up save files before replacing a build.

Save states are more fragile and may be incompatible between different builds or emulator/core versions. In-game saves are strongly recommended for long-term progress.

## Download and patching

Download the ZIP package from the [v0.1.11-beta release page](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.11-beta). It contains the xdelta patch, checksum manifest, English CUE file, and patching scripts/instructions for macOS, Linux/Steam Deck, and Windows. The xdelta patch has been decoded against the required Japanese source and reproduces the published target checksum exactly. This full patch requires the Japanese source, not a previous English BIN. It remains a work-in-progress test candidate, not a final-quality release.

The patch requires a legally obtained Japanese Track 01 with this SHA-256 checksum:

`1a9ce56a4746320f326fcc1269442ecf1917893d0e9feaf75030e98012d88b0f`

No ROM, disc image, BIOS, or unauthorized copyrighted game asset will be distributed by this repository.
