# st-term-colors
This is a collection of colorscheme patches for [st terminal] (st.suckless.org).
All of them are made using [terminal.sexy] (terminal.sexy) web app.
Works for st version 0.6.

## Installation
If using [ABS] (https://wiki.archlinux.org/index.php/Arch_Build_System) like what I do, simply add these colorscheme into your PKGBUILD.
For example, to use [gruvbox] (https://github.com/morhetz/gruvbox)-dark colorscheme, do:
1. Add the corresponding `.diff` to the `source` array in the PKGBUILD
2. Append `patch -p1 < $srcdir/$pkgname-$pkgver-gruvbox-dark.diff` to the `prepare()` function
3. `updpkgsums >> PKGBUILD`
4. `makepkg -si`
