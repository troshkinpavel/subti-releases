# Subti — releases

**[Subti](https://subti.app) is a macOS menu bar app that makes the subtitles in VLC clickable, so you
can look up a word in the film you are already watching and keep it.**

Hold <kbd>⌥</kbd> and click a word. The film pauses, and a model running on your own Mac translates
it — reading the whole subtitle line, so it knows the difference between *count* and *count on*.
Close the card and playback continues. Every word you looked up is waiting in History afterwards.

This repository is the public home for **Subti's releases and changelog**. The app's source code is
not public. What you find here is the release notes, the version and build numbers, and the SHA-256
checksums for every published build, next to the same DMG that subti.app serves — so you can check
what you downloaded against a second, independent source.

## Download

**[subti.app](https://subti.app)** — always the current version.

Builds are also attached to each entry under [Releases](https://github.com/troshkinpavel/subti-releases/releases)
on this page. GitHub is a mirror and a place to verify checksums; it is not where Subti checks for
its own updates. The canonical sources are:

- https://subti.app
- https://downloads.subti.app

## Requirements

- **macOS 14** or later
- **[VLC](https://www.videolan.org) 3.0** or later, in `/Applications`
- **Apple silicon**, to run a translation model inside the app. An Intel Mac can use Ollama or
  macOS Translate instead.
- **Accessibility** and **Automation** permission, which the app asks for at first launch. They let
  it follow VLC's window and see the ⌥ key. Nothing outside VLC's window is read.

## What it does

- **Clickable subtitles over VLC.** Subti draws the subtitle track itself, on top of the film you
  already have. No special build of VLC, no re-encoding, no separate video player. Clicks pass
  through to VLC unless you are holding the key.
- **A word, or a whole phrase.** Click one word, or drag across several, and it answers about the
  expression you actually chose — *take it for granted*, not *granted*.
- **Translated in context.** The model is given the entire line, so it can tell you which words the
  expression covers and what it means where it stands.
- **The line's own audio.** The card plays those seconds cut from the film, in the actor's voice, on
  the audio track VLC is playing.
- **History, then a dictionary.** Every lookup is kept while you watch. Afterwards you promote the
  ones worth learning and delete the rest.
- **Spaced repetition.** Review the words that are due, or export them — plain JSON, or an Anki deck
  that carries the line, its audio and the frame it was said over.
- **Any language pair.** 76 languages. English → Russian is only the default.
- **Subtitles from the file or beside it.** External `.srt`, `.vtt`, `.ass` and `.ssa`, and embedded
  text tracks by way of ffmpeg, which the app can install for you.

## Privacy

Subti runs on your Mac and keeps what it learns there. Translation happens locally — a model inside
the app, Ollama, or macOS's own translator. The films you watch, the words you look up and the
dictionary you build never leave the machine: no account to watch with, no telemetry, no server that
sees your library.

The app talks to subti.app for two things only: checking for a new version, and activating a licence
key. Neither carries anything about what you are watching. This is described in full in the
[privacy policy](https://subti.app/privacy).

## Licence

One purchase, no subscription. **A licence is for one person and can be active on up to 2 Macs at a
time** — a desktop and a laptop, typically. Settings shows where a Mac stands and frees its place
when you replace it. Updates are included and the licence does not expire.

Full terms: [subti.app/terms](https://subti.app/terms).

## Changelog

[CHANGELOG.md](CHANGELOG.md) in this repository, and [subti.app/changelog](https://subti.app/changelog).

## Support and issues

- Something not working? Start with [subti.app/support](https://subti.app/support) — the common
  problems and their fixes are there.
- Still stuck, or want to report a bug: email **[support@subti.app](mailto:support@subti.app)**, or
  open an [issue](https://github.com/troshkinpavel/subti-releases/issues) on this repository. See
  [SUPPORT.md](SUPPORT.md).
- Found a security problem? Please report it privately: [SECURITY.md](SECURITY.md).
