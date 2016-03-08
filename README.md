st-term-colors
==============

This is a collection of colorscheme patches for [st terminal] (st.suckless.org), made using [terminal.sexy] (terminal.sexy) web app. Works for version 0.6.

Installation
------------

If using [ABS] (https://wiki.archlinux.org/index.php/Arch_Build_System) like me, simply add these colorscheme into your PKGBUILD.
For example, to use [gruvbox] (https://github.com/morhetz/gruvbox)-dark colorscheme, do:

1. Add the corresponding `.diff` to the `source` array in the PKGBUILD
2. Append `patch -p1 < $srcdir/$pkgname-$pkgver-gruvbox-dark.diff` to the `prepare()` function
3. Run `updpkgsums >> PKGBUILD` to update the pkgsums, and then followed by `makepkg -si`
4. Profit
