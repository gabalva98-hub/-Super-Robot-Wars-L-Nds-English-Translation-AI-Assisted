# Super Robot Wars L — English Fan Translation

An unofficial, free English fan translation of **Super Robot Wars L** for Nintendo DS, presented by **Gyasuke & Wakabayashy Workshop**.

The translation is distributed through an **offline HTML patcher**. The game itself is not included. You must provide your own clean Japanese game dump.

**Current release:** 0.9.0 (cumulative English release; internal build FB97 ASCII P10)  
**Last updated:** November 18, 2026  
**Language:** English

## What's included

- English story translation and editorial text reflow. The earlier Story62 review covered **26,677 dialogue boxes in 59 internal story units** (source banks and branches, not 59 playable stages).
- English combat dialogue across the battle-text banks, including fixes for nameplates, dynamic markers, and line wrapping.
- An English **SUPER ROBOT WARS** title graphic preserving the original **L** emblem.
- English menus, pilot and unit names, weapon names, Spirit commands, abilities, and many terrain and location labels.
- A variable-width font (VWF), improved Latin-letter spacing, dialogue rendering, and text-buffer handling.
- **Native one-byte ASCII reading** in the relevant game engine paths, allowing better use of the existing text storage instead of expanding every Latin character into a two-byte Japanese encoding.
- Expanded and reviewed names for pilots, units and weapons, along with updated skill and Spirit descriptions. Some short list labels remain abbreviated to fit their display areas; the full-name fields are retained where appropriate.
- Improved unit-name consistency, including **Jack Smith**, and more consistent labels for transformable units and their variants (such as Taurus, Gaia Gundam and Murasame).
- Improved horizontal layout in **Unit Stats**: compact unit-name formatting and a corrected starting position for scaled unit names so that their first letters do not overlap the unit icons.
- Adjusted **Spirit** label alignment to move those names slightly left without changing their descriptions or icons.
- Accumulated earlier fixes for NUNS, VF-171 variants, Strike Freedom, Dancouga Nova MAXGOD, Talisman's **Tail Kingdom Max** weapon, and other reported names.
- Previous battle and UI corrections, including the FB95 dynamic-marker fix in battle bank 176, FB96's reflow of **547 battle interventions** in banks 0 and 174 (removing **581 extra line breaks**), and FB97's **Enemy PU**, **All Foes** and **Iczer C/S** labels. The Iczer **Combine** and **Separate** commands are retained.
- A standalone patcher for compatible desktop and Android browsers that works offline and does not upload your ROM.

## Installation

1. **Back up** your original Japanese `.nds` file and existing `.sav`, if any.
2. Download the **0.9.0** patcher.
3. Open `SRWL 0.9.0 FB97 P10.html` in a compatible browser on your computer or Android device.
4. Select your **clean, unmodified Japanese Super Robot Wars L ROM** (`.nds`). Do not select a ZIP archive or an already patched ROM.
5. Click **Apply Patch**, then save the English-patched `.nds` file.
6. Launch the generated ROM in a compatible emulator or on your own hardware.
7. To continue an existing save, back it up first and, if required by your emulator or flashcart, match the `.nds` and `.sav` base filenames.

**Important:** Version **0.9.0 is cumulative**. Always apply it to the original Japanese ROM. **Do not apply it over 0.8.0, FB97, P9, or any other patched version.**

### Required ROM

The patcher expects this Japanese dump:

| Property | Value |
| --- | --- |
| Size | `134,217,728` bytes (128 MiB) |
| CRC32 | `82804748` |

The source filename may differ, but its contents must match the required checksum.

### Expected 0.9.0 result

| Property | Value |
| --- | --- |
| Suggested filename | `Super_Robot_Wars_L_FB97_ASCII_P10_EN.nds` |
| Size | `134,217,728` bytes |
| CRC32 | `C1D747FB` |
| SHA-256 | `dffe76e45f2681b4ae15d64d86515d7a86a1fffa2b2a57e2da0849e5c44930af` |

The filename still contains **FB97 ASCII P10** because that is the internal technical build name. The public release version is **0.9.0**.

## Testing and project status

**Full-playthrough tester: Harrier Du Bois**

Harrier Du Bois reported completing a playthrough of an earlier build, following these route choices:

- Rescue the Mobile Suits
- Defend JUDA
- Help the Minerva
- Patrol Space

Harrier also repeatedly tested combination attacks against the final boss and **did not encounter the previously reported Heero Yuy portrait/name issue** during those tests.

Many thanks to Harrier Du Bois for completing the playthrough and providing detailed feedback. A completed playthrough of an earlier build does **not** certify every route or every technical change introduced in 0.9.0.

### 0.9.0 validation

The cumulative 0.9.0 patch passed structural checks and independent binary reconstruction. The HTML patcher applied to the supported clean Japanese ROM produced output **byte-identical** to the verified P10 build, matching the CRC32 and SHA-256 above.

The unit-name overlap was reproduced in **melonDS 1.1** by loading a Chapter 37 save from the title-screen **Load** option, opening **Unit Stats**, and inspecting the list. All 12 pages were reviewed on P9 to locate the problem. On P10, targeted emulator comparisons confirmed that scaled names, including **Taurus (Sanc K.)(MA)**, begin in the intended column and fit within the tested row. Spirit alignment was also checked on a pilot's status screen in an earlier ASCII build.

**Still pending:** a complete visual pass of all 12 Unit Stats pages specifically on P10, and full real-hardware testing of 0.9.0. Earlier fixes, including the FB97 UI labels, have not all received individual visual confirmation.

## Known limitations and bug reports

- Some short unit, ability, Spirit, terrain and interface labels remain abbreviated because different Nintendo DS screens have different width limits.
- Additional Unit Stats configurations and especially long names may still reveal clipping or alignment issues; the P10 display fix has had targeted, not exhaustive, visual testing.
- The earlier report of **Heero Yuy appearing during other pilots' combination attacks or new-attack events** was not reproduced in Harrier's final-boss tests. Other event triggers have not been exhaustively checked; please report any recurrence.
- Other route choices, hidden or optional events, attack-unlock scenes, and different emulator or hardware setups may expose additional issues.

If you encounter a crash, incorrect portrait, untranslated name, clipped dialogue or other UI problem, please open an issue in this GitLab project and, if possible, include:

- The **patch version** (**0.9.0**) and emulator or hardware used.
- The **chapter**, route choices, and relevant units or pilots.
- The **last visible dialogue** or the specific screen or attack involved.
- A screenshot or short video; a crash dump can also help when available.

Please back up your save before reproducing a problem. **Do not upload copyrighted ROM files** in issue reports.

## Credits

- **Project and patch presentation:** Gyasuke & Wakabayashy Workshop

### Testers

- **Harrier Du Bois** — Completed a full playthrough of an earlier build, taking the Rescue the Mobile Suits, Defend JUDA, Help the Minerva and Patrol Space routes; repeatedly tested combination attacks against the final boss.
- **Theoldnile** — Playtester who provided feedback for Super Robot Wars L.

A huge thank you to Harrier Du Bois, Theoldnile, and everyone who has provided screenshots, bug reports, save files and testing feedback. Your help has been essential to improving this translation.

## Legal notice and distribution

This is an **unofficial, non-commercial fan translation**. It is not affiliated with, sponsored by, or endorsed by Bandai Namco or the original rights holders. All original game content, trademarks and characters remain the property of their respective owners.

**The patch is free. It must not be sold or placed behind a paywall.** If you paid someone for this patch, that payment was not authorized by this project.

No game ROM or BIOS is distributed here. You are responsible for obtaining and using your own game files in accordance with applicable laws.

---

Thank you for playing **Super Robot Wars L** in English!
