<a href="https://github.com/leehowardblair/PGATeeTimeBuilder-Releases/blob/main/logo_header.png">
  <img src="https://github.com/leehowardblair/PGATeeTimeBuilder-Releases/blob/main/logo_header.png" width="150" alt="PGA Tee Time Builder logo">
</a>

# PGA Tee Time Builder v1.2.0

## ✨ Highlights
- Fully signed and notarized Universal macOS release for Apple Silicon and Intel Macs.
- Intel macOS Monterey startup compatibility is now included in the main macOS app (a.k.a "💃 Taylor's Version!").
- Choose the finished output files you need: **Excel**, **PDF**, and on macOS, **Numbers**.
- The completion screen carries tournament branding and clickable output-file links.

## 🖥️ Intel macOS Monterey startup reliability
- On affected Intel macOS 12 Monterey machines, the app now prepares a private execution directory.
- The signed macOS bundle includes the companion Hardened Runtime entitlement required by that Intel libffi startup path.
- This startup workaround runs only in an **Intel x86_64 macOS process**. Windows and native Apple Silicon retain their existing application startup behavior.
- The compatibility build was validated by a successful direct launch on the affected Intel Monterey machine.

## 🚨 Live Round 1 / Round 2 field updates
- The app first checks the official **Field Updates** page for explicitly named pre-round substitutions, including `WD / IN` and `replaced by` notices.
- A named replacement is always presented for operator confirmation before it changes the PDF-derived tee sheet.
- Replacement prompts and red `UNKNOWN - WD REPLACEMENT` fallbacks are limited to the **AM or PM wave currently being exported**.
- Standard paired Round 1 / Round 2 PDFs use the round-aware page order: **Round 1 page 1 = AM / page 2 = PM; Round 2 page 1 = PM / page 2 = AM.**
- Notices that clearly state a player withdrew **after Round 1** are excluded from pre-round replacement matching.

## 🐞 Fixes
- Removed the dark label highlighting from the light Settings window.
- Improved created-file behavior when a previous Excel or PDF output is open: the existing file is preserved and a newly timestamped output is written instead.
- Completion validation messaging is scoped to the file being created rather than the opposite wave.
- The macOS release pipeline now verifies the Intel Monterey compatibility entitlement after codesigning.

## 📝 Notes
- Live reconciliation runs for Rounds 1 and 2 only. The app never guesses an alternate; when a direct official replacement cannot be confirmed or is declined, the exact slot is shown in red as `UNKNOWN - WD REPLACEMENT`.
- Excel remains selected by default. Native Numbers output requires Apple Numbers and may request Automation permission once.
- This is a full **v1.2.0** update from v1.1.5; installed v1.1.5 copies should see it through Check for Updates after `latest.json` is published.

---

# 📦 Installation

**Windows**  
`PGA_TeeTime_Builder_Setup_v1.2.0.exe`

**macOS**  
`PGA_TeeTime_Builder_macOS_v1.2.0.zip`

© 2026 Lee Blair. All Rights Reserved.
