# CeGCC-9-PKGBUILDs

Arch Linux PKGBUILDs for [CeGCC 9](https://max.kellermann.name/projects/cegcc/) by MaxKellermann.

Partially based on [cegcc-build](https://github.com/MaxKellermann/cegcc-build) and PKGBUILDs for `mingw-w64-toolchain`.

## Bootstrap sequence

Each step means build and install (i.e. `makepkg -si` or `makepkg` then `pacman -U`).

```
binutils -> gcc-base -> mingwrt -> w32api -> gcc (overwrites gcc-base)
```
