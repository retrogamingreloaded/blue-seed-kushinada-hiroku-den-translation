# Blue Seed: Kushinada Hirokuden — English Translation

English fan translation and preservation project for **Blue Seed: Kushinada Hirokuden** on Sega Saturn.

*** STILL IN BETA - EXPECT SOME ISSUES ***

## Project status

A complete English candidate build has now been assembled.

- 5,157 unique text entries AI translated
- Dialogue, menus, and residual game text included
- All 79 detected interactive choice menus passed source and rebuilt-layout validation across 178 locations
- Automated checks cover dialogue glyph bounds, embedded text commands, and interactive-choice layout; they do not replace manual proofreading
- The rebuilt disc image boots successfully with the Beetle Saturn core
- The complete build was deployed and launched successfully on a Steam Deck with RetroArch/Beetle Saturn on October 11, 2026
- The October 12, 2026 beta refresh fixes 27 audited choice menus, chapter 2 text artefacts, and two missing half-width capitals
- The October 13, 2026 beta refresh fixes the garbled Options/Pad Controls screen and its controller-button labels
- Version 0.1.4-beta adds punctuation/font corrections, fixes embedded-command text artefacts, translates the Load Data screen and all 13 chapter-title images, and improves six chapter 2 dialogue blocks
- The v0.1.4-beta build was deployed to Steam Deck with its installed checksum verified; confirmation of every corrected screen in-game remains part of beta playtesting
- Version 0.1.5-beta corrects hippo-underwear references, harmonizes Yoshiki's name, fixes Kasumi Kusunoki's gender and the chapter 3 investigation dialogue, and removes stray opening apostrophes
- The v0.1.5-beta build was deployed with its installed checksum verified and all 125 existing Blue Seed save/state hashes unchanged; further semantic proofreading remains in progress
- Full-game playtesting, proofreading, and manual visual QA are still in progress

A ROM-free beta patch is now publicly available: **[Complete English Patch v0.1.5-beta](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.5-beta)**.

This remains a pre-release build while full-game proofreading and visual QA continue.

## Save compatibility

Sega Saturn backup-memory saves can be retained between translation builds when the same RetroArch content filename and core are used. Always back up save files before replacing a build.

Save states are more fragile and may be incompatible between different builds or emulator/core versions. In-game saves are strongly recommended for long-term progress.

## Download and patching

Download the complete ZIP package from the [v0.1.5-beta release page](https://github.com/retrogamingreloaded/blue-seed-kushinada-hiroku-den-translation/releases/tag/v0.1.5-beta). It contains the xdelta patch, checksum manifest, English CUE file, and patching scripts/instructions for macOS, Linux/Steam Deck, and Windows. The macOS apply script has been tested against the required source and reproduces the published target checksum exactly.

The patch requires a legally obtained Japanese Track 01 with this SHA-256 checksum:

`1a9ce56a4746320f326fcc1269442ecf1917893d0e9feaf75030e98012d88b0f`

No ROM, disc image, BIOS, or unauthorized copyrighted game asset will be distributed by this repository.
