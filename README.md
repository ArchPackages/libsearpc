# libsearpc — Arch Linux package

Packaging for [libsearpc](https://github.com/haiwen/libsearpc) 3.3.0, the C RPC
framework used by Seafile.

## Fork provenance

Forked from the AUR package **libsearpc**:

<https://aur.archlinux.org/packages/libsearpc>  
<https://aur.archlinux.org/libsearpc.git>

Originally packaged by **eolianoe** and contributors, and currently maintained
on the AUR by **thealchemist**. Many thanks to them and to the Seafile
developers at Haiwen for the upstream project.

This fork is maintained by **Miroslav Pavleski** <miroslav@pavleski.net>.

## Why this fork

It provides a pinned build of the Seafile dependency for the
[ArchPackages pacman repository](https://github.com/ArchPackages/archrepo),
without the CI build depending on a moving AUR clone.

The package keeps the AUR epoch (`2:3.3.0-5`). Build with `makepkg -f`;
install with `pacman -U`.
