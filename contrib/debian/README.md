
Debian
====================
This directory contains files used to package thecashd/thecash-qt
for Debian-based Linux systems. If you compile thecashd/thecash-qt yourself, there are some useful files here.

## thecash: URI support ##


thecash-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install thecash-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your thecashqt binary to `/usr/bin`
and the `../../share/pixmaps/thecash128.png` to `/usr/share/pixmaps`

thecash-qt.protocol (KDE)

