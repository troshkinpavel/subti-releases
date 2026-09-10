# releases/

One file per published version: its release notes, the build number, and the SHA-256 of each
artifact subti.app serves for it.

**The builds themselves are not in this directory.** They are attached to their entry under
[Releases](https://github.com/troshkinpavel/subti-releases/releases), and served from
[downloads.subti.app](https://downloads.subti.app). This directory is the plain-text record beside
them: readable in a browser, in `git log`, and in a diff — so a checksum published on the day of a
release can be seen not to have changed since.

Nothing here is what Subti updates itself from. The app's update feed is served by subti.app, and
GitHub is a mirror.
