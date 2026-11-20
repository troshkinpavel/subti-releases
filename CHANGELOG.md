# Changelog

Public release notes for [Subti](https://subti.app). Same words as
[subti.app/changelog](https://subti.app/changelog), which is where they are written; this file
mirrors them after each release is published.

Each entry lists the version, the build number and the SHA-256 of the DMG that subti.app serves, so
a download can be checked against a second source. The app itself is attached to its entry under
[Releases](https://github.com/troshkinpavel/subti-releases/releases), with a `SHA256SUMS.txt`:

```bash
shasum -a 256 -c SHA256SUMS.txt
```

---

## 0.3.7 — build 10

*21 November 2026 · requires macOS 14.0 or later*

**Open History from VLC — full screen included — and export History straight from its toolbar.**

### Improved

- Open History's shortcut needs ⌥ or ⌃ now that it works in every app — a ⌘-only one would take
  ⌘C or ⌘W away from all of them. A ⌘-only shortcut set in 0.3.6 goes back to ⌥H.

### Fixed

- **The History shortcut works while you watch.** ⌥H — or your own shortcut — opens History with VLC
  in front, full screen included, without opening Subti's menu first. Before, it only worked while
  that menu was open.
- The shortcut is the same physical key under any keyboard layout, Russian and Greek included.
- History opens over a full-screen film, on the Space you are watching, and on the History tab.
- **History's Export menu was missing in 0.3.6.** It is now on History's toolbar: Export Selected…,
  Export All for This Movie… and Export List…, and Export… appears when you tick rows in Select mode.
  Nothing needs adding to the Dictionary first.

**SHA-256** · `Subti-0.3.7.dmg` `22451b7eee2d1485dd7a36bcda90b212311fca7e9c5cc5c944b067a8479d2dee`
## 0.3.6 — build 9

*17 November 2026 · requires macOS 14.0 or later*

**Export a whole film's History in one go, however many words it holds, and choose your own History shortcut.**

### Added

- **Export All for This Movie…** in History: every word and phrase you looked up in a film, written
  out with its line, timestamp and translation — no need to add them to the Dictionary first.
- Choose your own shortcut for **Open History** in Settings ▸ Shortcuts, with Reset to Default.

### Improved

- History's JSON export now keeps everything History records: how often you looked a word up, which
  translator answered, where the line starts and ends, the audio track, and whether the word is in
  your Dictionary.
- Two films with the same file name in different folders are kept apart in the film filter.

### Fixed

- History no longer stops at 500 entries. A film with more lookups than that showed only some of
  them — or none at all, once newer films had filled the first 500 — and exported only what it showed.

**SHA-256** · `Subti-0.3.6.dmg` `a23b63e16fb1ba68c8611cf7f734c821a98c12e760b7611259e7ceb7f9710340`
## 0.3.4 — build 7

*10 September 2026 · requires macOS 14.0 or later*

**Licence keys issued by subti.app are accepted by this build.**

### Fixed

- A licence key bought from subti.app now verifies. This build carries the signing key those keys
  are made with; earlier ones checked against an older key and refused every one of them.

**SHA-256** · `Subti-0.3.4.dmg` `6a4303122d4e8a9b381d2b875776dda2ed91a3a20edb6e4adade287b98201a82`
