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

The notes below are the original, in Bulgarian.

---

# Слоят Wine за RigDesk

Тук лежи един файл: `wine-x86_64.tar.xz` — Wine, компилиран за телефон, който
[RigDesk](https://rigdesk.app) си сваля сам при първото пускане.

Тук **не се пише** Wine и тук няма как да се строи. Това е складът, от който
приложението се обслужва; работилницата е другаде.

## Какво е вътре

Wine 11.3, компилиран за `x86_64-linux-android28`, плюс библиотеките, които
се отварят по време на работа. Разпакетиран е около 430 MB.

## Лиценз

Wine е чужд свободен код под **LGPL-2.1**, писан от 1993 г. от общността.
Лицензите на всичко вътре пътуват в самия архив, в папка `licenses/`.

Изходният код е публичен и не е променян по същество:

- upstream: <https://gitlab.winehq.org/wine/wine> — клон `wine-11.3`
- кръпките за Android/bionic: <https://github.com/GameNative/wine>

LGPL иска този слой да може да се подмени с друг. Може: RigDesk приема слоя и
като обикновен файл — в прозореца *Windows* има избирач, с който се посочва
собствен архив вместо този.
