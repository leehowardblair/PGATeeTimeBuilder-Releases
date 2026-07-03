<a href="https://github.com/leehowardblair/PGATeeTimeBuilder-Releases/blob/main/logo_header.png">
  <img src="https://github.com/leehowardblair/PGATeeTimeBuilder-Releases/blob/main/logo_header.png" width="150" alt="PGA Tee Time Builder logo">
</a>

# PGA Tee Time Builder v1.1.5

## ✨ Highlights
- Choose the finished output files you need: **Excel**, **PDF**, and on macOS, **Numbers**.
- The completion screen now carries tournament branding and clickable links
- Added print-ready PDF tee sheets
- Improved native Numbers export on macOS with better first-use readiness

## 🚨 Live Round 1 / Round 2 field updates
- The app first checks **Field Updates** page for explicitly named pre-round substitutions, including `WD / IN` and `replaced by` notices.
- A named replacement is always presented for operator confirmation before it changes the PDF-derived tee sheet.
- Replacement prompts and red `UNKNOWN - WD REPLACEMENT` fallbacks are limited to the **AM or PM wave currently being exported**. 
- Standard paired Round 1 / Round 2 PDFs now use the correct round-aware page order: **Round 1 page 1 = AM / page 2 = PM; Round 2 page 1 = PM / page 2 = AM.**
- Notices that clearly state a player withdrew **after Round 1** are excluded from pre-round replacement matching.

## 🐞 Fixes
- Removed the dark label highlighting from the light Settings window.
- Improved created-file behavior when a previous Excel or PDF output is open: the existing file is preserved and a newly timestamped output is written instead.
- Completion validation messaging is scoped to the file being created rather than the opposite wave.

## 📝 Notes
- Live reconciliation runs for Rounds 1 and 2 only. The app never guesses an alternate; when a direct official replacement cannot be confirmed or is declined, the exact slot is shown in red as `UNKNOWN - WD REPLACEMENT`.
- Excel remains selected by default. Native Numbers output requires Apple Numbers and may request Automation permission once.
- **Known issue:** the separate Intel macOS Monterey startup investigation is not included in v1.1.5 and remains planned for v1.2.0.

---

# 📦 Installation

**Windows**  
`PGA_TeeTime_Builder_Setup_v1.1.5.exe`

**macOS**  
`PGA_TeeTime_Builder_macOS_v1.1.5.zip`

© 2026 Lee Blair. All Rights Reserved.
