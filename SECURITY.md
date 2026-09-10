# Security

If you have found a security problem in Subti, please tell me privately first.

**Email [support@subti.app](mailto:support@subti.app)** with `security` in the subject line. Please
do not open a public issue, post the details anywhere public, or describe the problem in a pull
request until it has been fixed and a build carrying the fix has shipped.

Not because the report is unwelcome — the opposite. Subti is installed on other people's Macs, and a
description in the open reaches whoever wants to use it before it reaches the people who need to
update.

## What helps

- What the problem lets someone do, and roughly how.
- The Subti version and build (the menu bar shows both), and your macOS version.
- Steps to reproduce it, if you have them.

You do not need a proof of concept. A clear description of the weakness is enough to start.

## What happens next

- I will confirm I have your report within **3 working days**.
- I will tell you whether it is a real problem, and what I intend to do, within **10 working days**.
- Once a fix has shipped, I will say so, and credit you in the release notes if you would like that.

Subti is one person's work, not a company with a rota, so please allow for that in the timings above.
If you have not heard back in a week, send the email again — it went astray rather than ignored.

## Scope

This repository holds no application source code. It exists to distribute builds and publish their
checksums. Reports are welcome about:

- The Subti app itself.
- subti.app and downloads.subti.app, including licence activation and the update feed.
- The artifacts published here — a checksum that does not match, a build that is not signed by the
  expected team, anything suggesting a download has been tampered with.

Every published build is signed with an Apple Developer ID and notarized by Apple, and every release
lists its SHA-256 so you can check the copy you have.

## Out of scope

Reports produced by an automated scanner with no working attack behind them, missing hardening that
has no exploitable consequence, and problems in VLC, Ollama or macOS itself — those belong with
their own projects.
