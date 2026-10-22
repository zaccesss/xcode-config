# Changelog

All notable changes to this project are recorded here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Versioning follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Added

- A screenshot of the editor in the Zacess Deep Contrast Dark theme.

## [0.0.1] - 2026-10-22

### Added

- Initial release: `prefs.txt` with the Xcode preferences read from Xcode 27.1: the light and dark
  editor themes for Xcode 26 and earlier, the Xcode 27 theme setting as hex data, the key bindings
  set, predictive code completion off and automatic string catalog comments off
- `theme/` with the eight Zacess Xcode themes from Zacess Themes and Zacess Deep Contrast Dark in
  Xcode 27's `.xcworkspacecolortheme` format, so no manual import is needed for it
- `KeyBindings/Default.idekeybindings`, the default key bindings set
- `apply.sh`, which copies the themes and the key bindings file, writes each recorded preference
  that differs, backs up the defaults domain before the first write, refuses to run while Xcode is
  open and takes `--dry-run`
- Setup and reference guides explaining every key and the Xcode 27 theme import
- `ACCESSIBILITY.md` covering the themes, the editor font and the keyboard
- CI that checks `prefs.txt` and the key bindings file and runs `bash -n` and shellcheck on the
  script, plus markdown lint
