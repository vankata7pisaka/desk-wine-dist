# Wine for RigDesk — the built layer

This is the Wine layer that **[RigDesk](https://rigdesk.app)** downloads by itself the first
time you set up Windows programs on an Android phone. One file lives here,
`wine-x86_64.tar.xz`, attached to the [releases](https://github.com/vankata7pisaka/desk-wine-dist/releases).

- **What it is:** Wine 11.3 compiled for `x86_64-linux-android28`, plus the libraries it opens
  at run time. box64 translates it to ARM on the phone — no root, no Linux image.
- **Where it is built:** in the open, from public source, in
  [`desk-wine`](https://github.com/vankata7pisaka/desk-wine) — the build recipe and the patches.
- **Licence:** Wine is LGPL-2.1. The licences of everything inside travel in the archive, under
  `licenses/`. LGPL asks that this layer can be swapped for another one, and it can: the
  *Windows* window in RigDesk has a picker for your own archive.

**RigDesk** — desktop mode for any Android: [rigdesk.app](https://rigdesk.app) ·
[download](https://rigdesk.app/download) · [guide](https://rigdesk.app/guide)

## What is inside

Wine 11.3 compiled for `x86_64-linux-android28`, plus the libraries it opens at run time.
About 430 MB unpacked. Wine is not written here and is not built here — this repository only
serves the finished file; the build lives in [`desk-wine`](https://github.com/vankata7pisaka/desk-wine).

The source is public and not changed in substance:

- upstream: <https://gitlab.winehq.org/wine/wine> — branch `wine-11.3`
- the Android/bionic patches: <https://github.com/GameNative/wine>
