# st-bandithijo

The Simple Terminal with BanditHijo's Personal Preference Patches (with Binary included).

**st version**: 0.8.4

![st-bangithijo image](https://i.postimg.cc/tg7fD9wQ/st-bandithijo.png)

## 📦 Patches Included

0. [appsync](https://st.suckless.org/patches/sync/)
0. [bold-is-not-bright](https://st.suckless.org/patches/bold-is-not-bright/)
0. [border-resize](https://t.me/sucklesscode/9005)
0. [boxdraw](https://st.suckless.org/patches/boxdraw/)
0. [cursorblink](https://st.suckless.org/patches/blinking_cursor/)
0. [exteralpipe](https://st.suckless.org/patches/externalpipe/)
0. [font2](https://st.suckless.org/patches/font2/)
0. [invert](https://st.suckless.org/patches/invert/)
0. [ligatures](https://st.suckless.org/patches/ligatures/)
0. [newterm](https://st.suckless.org/patches/newterm/)
0. [openclipboard](https://st.suckless.org/patches/open_copied_url/)
0. [scrollback](https://st.suckless.org/patches/scrollback/)
0. [undercurl](https://st.suckless.org/patches/undercurl/)
0. [universcroll](https://st.suckless.org/patches/universcroll/)
0. [w3m](https://st.suckless.org/patches/w3m/)
0. [workingdir](https://st.suckless.org/patches/workingdir/)
0. [xresources-livereload](https://github.com/nimaipatel/st/commit/144c1b2eec9adde37ad8a7b4e46c2725cf8fa41c?branch=144c1b2eec9adde37ad8a7b4e46c2725cf8fa41c&diff=unified)
0. [xresources](https://st.suckless.org/patches/xresources/)

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
0. For externalpipe patch, I use this script: [**st-urlopener**](https://github.com/thomas154/st-urlopener). Drop [**urlopener**](https://raw.githubusercontent.com/thomas154/st-urlopener/master/urlopener) to your `$PATH`. You can modify from those and make personal adjustments.

## ⌨️ Keyboard Shortcuts

*Under contruction...*


## 👷 Original Project

st is a simple terminal emulator (proviced by suckless project) for X which sucks less.

Official website: [st.suckless.org](https://st.suckless.org)

## 🤝 Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

## 🏛️ License

[LICENSE](https://raw.githubusercontent.com/bandithijo/st-bandithijo/master/LICENSE)
