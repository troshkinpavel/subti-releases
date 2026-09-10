# Changelog

Public release notes for [Subti](https://subti.app). Same words as
[subti.app/changelog](https://subti.app/changelog), which is where they are written; this file
mirrors them after each release is published.

Each entry lists the version, the build number and the SHA-256 of the DMG that subti.app serves, so
a download can be checked against a second source. The DMG for each version is attached to its entry
under [Releases](https://github.com/troshkinpavel/subti-releases/releases).

Verify a download:

```bash
shasum -a 256 ~/Downloads/Subti-0.3.4.dmg
```

---

## 0.3.4 — build 7

*10 September 2026 · requires macOS 14.0 or later*

**Licence keys issued by subti.app are accepted by this build.**

### Fixed

- A licence key bought from subti.app now verifies. This build carries the signing key those keys
  are made with; earlier ones checked against an older key and refused every one of them.

**SHA-256** · `Subti-0.3.4.dmg` `6a4303122d4e8a9b381d2b875776dda2ed91a3a20edb6e4adade287b98201a82`
