# st-bandithijo

The Simple Terminal with BanditHijo's Personal Preference Patches (with Binary included).

**st version**: 0.8.4

**st-bandithijo version**: 1.1, [changelog](https://github.com/bandithijo/st-bandithijo/releases/tag/v1.1)

![st-bangithijo image](https://i.postimg.cc/tg7fD9wQ/st-bandithijo.png)

## 📦 Patches Included

0. [appsync][1]
0. [bold-is-not-bright][2]
0. [border-resize][3]
0. [boxdraw][4]
0. [cursorblink][5]
0. [exteralpipe][6]
0. [font2][7]
0. [invert][8]
0. [ligatures][9]
0. [newterm][10]
0. [openclipboard][11]
0. [scrollback][12]
0. [undercurl][13]
0. [universcroll][14]
0. [w3m][15]
0. [workingdir][16]
0. [xresources-livereload][17]
0. [xresources][18]

## 🏗️ Install

~~This repository have binary file~~.

First, you need to make it with,

```sh
$ make
```

Just install it to your system with,

```sh
$ sudo make install
```

After installation complete, default st binary location is on **/usr/local/bin/st**.

I prefer using those location because every binary program that I compile by my self should be on user location.

## 🛠️ Modification/Configuration

### Via config.h

[config.h](https://raw.githubusercontent.com/bandithijo/st-bandithijo/master/config.h)

Afer modifying file config.h, you need to re-make the source code.

```sh
$ make
```

And don't forget to re-[install](#install) again.

### Via Xresources

```
St.font:        JetBrainsMono Nerd Font Bandit:pixelsize=10
St.foreground:  #D4D4D4
St.background:  #1E1E1E
St.cursorcolor: #D4D4D4
St.borderpx:    3
```

\* Please, go to [here](https://github.com/bandithijo/JetBrainsMonoNerdFontCompleteBandit-Medium), if you interested with font that I used.

## 🍿 Recomendations

0. Install [**libxft-bgra**](https://aur.archlinux.org/packages/libxft-bgra/)<sup>AUR</sup>, If st crashes when viewing emojis.
0. Define your fallback font for symbol/glyph/emoji on `font2[]`. This repo defines [**ttf-octicons**](https://aur.archlinux.org/packages/ttf-octicons/)<sup>AUR</sup>, [**ttf-joypixels**](https://archlinux.org/packages/community/any/ttf-joypixels/).
0. For externalpipe patch, I use this script: [**st-urlopener**](https://github.com/thomas154/st-urlopener). Drop [**urlopener**](https://raw.githubusercontent.com/thomas154/st-urlopener/master/urlopener) to your `$PATH`. You can modify from those and make your personal adjustments.

## ⌨️ Keyboard Shortcuts

| Function                                                             | Keyboard Shortcuts                                                                                                                                                                                   | Patch                  |
| --                                                                   | --                                                                                                                                                                                                   | --                     |
| Scrolling screen up/down 1 page                                      | <kbd>Shift</kbd> (hold) + <kbd>PgUp</kbd> / <kbd>PgDown</kbd>                                                                                                                                        | [scrollback][12]       |
| Scrolling screen with mouse                                          | <kbd>Shift</kbd> (hold) + ScrollUp / ScrollDown                                                                                                                                                      | [scrollback-mouse][12] |
| Open new terminal with same directory (CWD)<br> as previous terminal | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd>                                                                                                                                                | [newterm][10]          |
| Invert terminal color                                                | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>X</kbd>                                                                                                                                                    | [invert][8]            |
| Border size increase/decrease                                        | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>I</kbd> (increase)<br><kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>D</kbd> (decrease)                                                                         | [border-resize][3]     |
| Open copied url to browser                                           | Copy URL with selection, <br>then passing to browser with <kbd>Alt</kbd> + <kbd>O</kbd>                                                                                                              | [openclipboard][11]    |
| Font resize increase/decrease/reset                                  | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>PgUp</kbd> (increase)<br><kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>PgDown</kbd> (decrease)<br><kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Home</kbd> (reset) |                        |

<br>

## 👷 Original Project

st is a simple terminal emulator (proviced by suckless project) for X which sucks less.

Official website: [st.suckless.org](https://st.suckless.org)

## 🤝 Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

## 🏛️ License

[LICENSE](https://raw.githubusercontent.com/bandithijo/st-bandithijo/master/LICENSE)

[1]: https://st.suckless.org/patches/sync/
[2]: https://st.suckless.org/patches/bold-is-not-bright/
[3]: https://t.me/sucklesscode/9005
[4]: https://st.suckless.org/patches/boxdraw/
[5]: https://st.suckless.org/patches/blinking_cursor/
[6]: https://st.suckless.org/patches/externalpipe/
[7]: https://st.suckless.org/patches/font3/
[8]: https://st.suckless.org/patches/invert/
[9]: https://st.suckless.org/patches/ligatures/
[10]: https://st.suckless.org/patches/newterm/
[11]: https://st.suckless.org/patches/open_copied_url/
[12]: https://st.suckless.org/patches/scrollback/
[13]: https://st.suckless.org/patches/undercurl/
[14]: https://st.suckless.org/patches/universcroll/
[15]: https://st.suckless.org/patches/w3m/
[16]: https://st.suckless.org/patches/workingdir/
[17]: https://github.com/nimaipatel/st/commit/144c1b2eec9adde37ad8a7b4e46c2725cf8fa41c?branch=144c1b2eec9adde37ad8a7b4e46c2725cf8fa41c&diff=unified
[18]: https://st.suckless.org/patches/xresources/
