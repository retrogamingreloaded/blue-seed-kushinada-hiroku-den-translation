# Changelog

## 0.1.5-beta — October 14, 2026

- Corrected two references to hippo underwear that had been translated as elephant shorts.
- Harmonized Yoshiki's name without English -kun/-san suffixes, as requested.
- Corrected Kasumi Kusunoki's gender in three references; removed an invented implication that she was deceased.
- Corrected the chapter 3 waking-up and investigation conversation: why she is in bed, how the others know her name, and who had whose background investigated.
- Removed two stray opening apostrophes and corrected who left the document on Yoshiki's desk.
- Updated 15 unique text IDs, preserving Japanese source columns and script controls.
- Retains the previous font, punctuation, load-screen and interactive-choice corrections.

Verification: 13 source/translation pairs pass; all 93 injected files verified against ISO readback; 79 text files, 3,159 messages and ten embedded command tails pass the glyph audit; 79 interactive choice IDs / 178 locations retain their commands and row geometry. The patch-application script reproduces the target exactly. Steam Deck installed checksum verified, content names/CUE retained, and all 125 pre-existing save/state hashes unchanged.

Patched Track 01 SHA-256:
`bc1a703c11510c55a195d73b9f38b91d5a79798ac8bef41070c8473266830ed7`

The required Japanese source is unchanged. Manual semantic proofreading continues: additional errors have been identified and are not all corrected by this focused release. Specific new screens still require in-game visual confirmation. No ROM, BIOS, audio track, game-art binary, or save is distributed.

## 0.1.4-beta — October 13, 2026

- Corrected Latin punctuation geometry: commas, periods, apostrophes, colons and semicolons; adjusted the capital T.
- Fixed missing-capital spacing in executable menus, including HP; Tea LIFE+5 now uses one ordinary space rather than right-aligned padding.
- Removed serialized translation residue and fixed ten dialogue-command text tails whose stale font indices caused visible garbage.
- Restored the full personal-record heading in a single condensed row; removed stray collection-heading chevrons and shortened an overflowing production credit.
- Translated the graphical Load Data heading and all thirteen chapter-title images on the save-loading screen. Future rebuilds now include these assets.
- Improved six chapter 2 dialogue blocks: natural cowardice teasing and response, an adapted coffer/coffin malapropism, the piece-of-cake idiom, and the enemy's dismissive threat.

### Verification

- 93 injected disc files verified by byte-for-byte readback.
- Glyph/command audit: 79 text files, 3,159 messages and ten embedded text tails; zero errors/warnings.
- Interactive choices: 79 IDs / 178 locations; selection commands and row geometry preserved.
- Six revised dialogue blocks checked against their actual rebuilt bitmaps and portrait-window limits.
- Package apply script reproduces the exact English Track 01 from the required Japanese source.
- Steam Deck deployment verified against the same target checksum. Existing content filenames and CUE retained; no saves replaced by deployment commands.

Required original Track 01 SHA-256:
`1a9ce56a4746320f326fcc1269442ecf1917893d0e9feaf75030e98012d88b0f`

Patched Track 01 SHA-256:
`e70c1ed871350e98a526c9a2d1cc443b854e5d99bacae5e722766c68f219500d`

This is still a beta. Automated validation and deployment do not prove every translation is accurate or every corrected screen is visually verified. Full-game proofreading and playtesting continue. Only patches and supporting documentation/scripts are distributed; no ROM, BIOS, audio tracks or game-art binaries are included.
