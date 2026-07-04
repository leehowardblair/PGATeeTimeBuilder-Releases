<a href="https://github.com/leehowardblair/PGATeeTimeBuilder-Releases/blob/main/logo_header.png">
  <img src="https://github.com/leehowardblair/PGATeeTimeBuilder-Releases/blob/main/logo_header.png" width="150" alt="PGA Tee Time Builder logo">
</a>

# PGA Tee Time Builder v1.2.2

## ✨ Revised PGA TOUR Media PDFs
- Before a tee sheet is built, the app now checks if there is a revised version.
- When a revised official PDF is available, the app clearly asks whether to use the **Revised PDF** or keep the **Original PDF** for that build.
- The revised file is never selected silently.
- A manual **PDF URL Override** remains available in the settings menu for any unfound PDF.

## 🧾 Official player-name validation
- Parsed player names are now checked against the selected tournament’s official PGA TOUR current-field JSON when it is available.
- Exact, unambiguous official aliases normalize inconsistent amateur markers, including `Preston Stout -a`, `Preston Stout (a)`, and `A Preston Stout` → `PRESTON STOUT -a`.
- Amateur status is preserved from the PGA TOUR Media PDF and always rendered at the end of the name as lowercase ` -a`.
- Weekend player/hometown text remains protected by exact token matching only; the app does not fuzzy-match or guess a player name.
- If the official field JSON is unavailable, the app retains the original PDF text and logs that the optional validation was skipped.

## 🐞 Retained fixes
- Includes the Windows and macOS updater-handoff repair from v1.2.1.
- Retains the Intel macOS Monterey startup compatibility fix from v1.2.0.
- Retains official R1/R2 Field Updates replacement prompts, AM/PM wave scoping, and round-aware R1/R2 PDF page mapping.

---

# 📦 Installation

**Windows**  
`PGA_TeeTime_Builder_Setup_v1.2.2.exe`

**macOS**  
`PGA_TeeTime_Builder_macOS_v1.2.2.zip`

© 2026 Lee Blair. All Rights Reserved.
