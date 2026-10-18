# Changelog

## 0.1.9-beta — October 18, 2026 — display-fix test candidate

- Removes decorative outer quotation marks from 32 unique interactive-choice texts (43 source-table occurrences), without changing choice commands or layout geometry.
- Shortens eight overlong embedded-command text tails to their original glyph-slot capacity, including the reported corrupted grass-screen dialogue.
- Limits eight statue inscriptions to two lines to avoid fourth-line overlap; includes recent source-checked dialogue and layout corrections.
- Static translation, glyph, choice-layout and disc-readback checks pass, and repeated MES/EXE rebuilding is byte-identical. The public xdelta patch decodes from the verified original Japanese Track 01 to the target SHA-256 below.
- **This exact image and the reported grass and statue screens have not yet been visually retested in-game.** Earlier boot/save tests apply to preceding candidates only.

Known remaining work: 2,180 model-unflagged passages still need independent proofreading; constable 大田原 / provisional Otawara (03188) remains uncertain. Full dialogue/choice-branch playtesting and final semantic approval are incomplete. This is a beta test patch, not a final release. No ROM, BIOS, original audio, game-art binary, save, private helper or internal TODO is distributed.

Patched Track 01 SHA-256:
`f975125538a0c3b4903e8231ee03913ca8905feff7e4a1f0855a1489fa03e2f7`

## 0.1.8-beta — October 17, 2026 — proofreading test candidate

- Incorporates 1,541 supervised correction IDs, including dialogue, menu and text-layout fixes made after v0.1.7-beta. These are candidate edits, not a count of severe bugs.
- The latest private build passed 48 automated checks and repeated identical MES/EXE rebuilding. The public xdelta patch was applied to the verified original Japanese Track 01 and reproduced the candidate byte for byte.
- This exact image has not yet been tested in-game. Earlier boot, save/reload and selected dialogue checks apply to preceding candidates only.

Known remaining work: 2,180 passages need independent proofreading; constable 大田原 / provisional Otawara (03188) remains uncertain. Full dialogue/choice-branch playtesting and final semantic approval are incomplete. This is a beta test patch, not a final release. No ROM, BIOS, original audio, game-art binary, save, private helper or internal TODO is distributed.

Patched Track 01 SHA-256:
`531b96c8d2b2442edd9e570cf6af52950b391becebda14088bd64d8b7a932960`

## 0.1.7-beta — October 16, 2026 — proofreading test candidate

- Incorporates 1,216 current candidate correction IDs, checked at 1,382 rebuilt locations. This cumulative proofreading snapshot includes source-based meaning/idiom corrections, restored puzzle/numerical clues, names, item descriptions, apostrophes and five compact choice menus with source selector positions preserved.
- Confirms Kazumi from the original game's pager; retains Yoshiki without honorific suffixes. The constable 大田原 is provisionally Otawara, not independently confirmed.
- All 15 baseline source validations, 13 scenario-prefix builds and an identical repeated MES/EXE rebuild pass. All 93 injected files pass disc readback. Menu checks cover 79 IDs / 178 locations; five compact menus have extra visible-option checks in 17 locations. All 51 targeted unit tests pass.
- The preceding 907-edit candidate passed local ordinary save → full emulator exit → cold start → load, chapter 1 load-screen and selected dialogue checks in Beetle Saturn. **The new 1,216-edit image has not been tested in-game or deployed to Steam Deck.** This is not evidence for all chapters or cross-device/state-version compatibility.
- Local vision-model testing found hallucinated defects and a missed choice-selection issue; no model result is accepted as visual certification.

Known remaining work: 2,694 model-unflagged passages need independent manual review; one name reading remains uncertain; full dialogue/choice-branch playtesting is incomplete. Final semantic approval is not granted. Published as an explicitly requested work-in-progress beta test patch, not a final release. No ROM, BIOS, original audio, game-art binary, save, private build/SCP helper or internal TODO is distributed.

Patched Track 01 SHA-256:
`e3a32fbe428c4c47c768487c86c6330530238482b68a0f150294440743271ebf`

## 0.1.6-beta — October 14, 2026

- Corrected all 24 previously confirmed remaining semantic errors; source-based review of adjacent dialogue, recurring names and item-acquisition notices expanded the update to 99 unique text IDs.
- Restored Izumo, Kumamoto and Yubari, the missing Mount Aso reference, the Kumamoto Station clue and late-spring timing.
- Corrected reversed subjects/objects in self-introductions, hostage threats, thanks, recognition dialogue and transfer orders; removed invented taunts and misread idioms.
- Corrected animal-pattern collection entries and acquisition notices: Okinawa rail, serow, flying squirrel, sea otter, squirrel, falcon, giraffe, elephant, giant tortoise and others.
- Harmonized Ryusen using the source's explicit phonetic spelling and corrected Ruri's Chinese transliteration. Yoshiki remains unchanged without -kun/-san.
- Restored Momiji's S+1 D+1 equipment bonuses and the sunlight vulnerability explanation.
- Fixed surplus collection chevrons, the incomplete TAC-return choice quote and the Shizuoka-shop choice wording without changing physical choice rows.
- Corrected nearby hotel, food and investigation dialogue, including cake, kelp tea and the Chief Cabinet Secretary's title.
- Retains all previous font, punctuation, load-screen and interactive-choice fixes.

Verification: all Japanese/source columns and script controls preserved; 99 changed IDs / 101 locations checked against actual rebuilt glyph sequences and window limits; all 93 injected files verified against ISO readback. Glyph audit covers 79 text files, 3,159 messages and ten embedded tails with zero errors/warnings. All 79 interactive-choice IDs / 178 locations preserve their selection commands and row geometry. The patch-application script reconstructs the target exactly. Installed Steam Deck checksum verified, content filenames/CUE retained and all 125 pre-existing save/state hashes unchanged. The previous installed ROM was backed up before replacement.

Patched Track 01 SHA-256:
`3bf388e6d552a52773ed76e3bae300475a3a166ea68471dcd97882d44c1a8331`

This closes the previous list of 24 confirmed errors, not full-game proofreading. Uncertain gameplay-rule interpretations have not been guessed. Manual review and in-game visual confirmation of every revised passage remain incomplete. Only the patch and supporting scripts/documentation are distributed; no ROM, BIOS, original audio or game-art binaries are included.

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
