# MLVWM

[![MLVWM System 7 Theme](/img/System7-640x360.png?raw=true)](#SCREENSHOTS)

## OVERVIEW

MLVWM (Macintosh-Like Virtual Window Manager) is an X11 window manager with a classic MacOS appearance. Its primary features include:

* Emulation of MacOS 7 & 8 menu bar & window decorations
* Optional multiple virtual desktops
* A main menu bar across the top of the screen, with:
  * Configurable global and per-application menus
  * Menu items trigger application functionality via keyboard shorcuts or commands
  * An icon menu which shows all windows and supports:
    * Switching desktops
    * Selecting, hiding, and showing windows
  * A balloon help menu
  * The ability to "swallow" small windows into the menu bar
* Windows which support:
  * Title bars with optional close, zoom, and shade buttons
  * Resize handle
  * Optional double-click to toggle window shade
  * Drag as solid window or just outline
* Balloon help which shows X window information
* Global keyboard shortcuts
* Numerous configuration options to tune functionality

## SCREENSHOTS

Default theme (System 7-like):

[![Default System 7 Theme](/img/System7-640x360.png?raw=true)](/img/System7-1920x1080.png)

`System8` theme (MacOS 8/9-like):

[![MacOS 8/9 Theme](/img/MacOS8-640x360.png?raw=true)](/img/MacOS8-1920x1080.png)

## INSTALLATION

### Building from Source

Build & installation currently still requires [imake](https://en.wikipedia.org/wiki/Imake) & make. While the original documentation says that `xmkmf -a` should work, we've found it's usually necessary to do the following:

    cd man && xmkmf && cd -
    cd sample_rc && xmkmf && cd -
    cd mlvwm && xmkmf && cd -
    xmkmf
    make && make install

### Package Managers

Native packages are provided on some operating systems, including:

* OpenBSD: `pkg_add mlvwm`
* NetBSD: `pkg_add mlvwm`
* Arch Linux: [Arch User Repository (AUR)](https://wiki.archlinux.org/title/Arch_User_Repository)
* NixOS

For an up-to-date list of packaged versions, see [mlvwm on Repology](https://repology.org/project/mlvwm/versions).

[![Packaging status](https://repology.org/badge/vertical-allrepos/mlvwm.svg)](https://repology.org/project/mlvwm/versions)

## CONFIGURATION

While some sample configuration files are included in the `sample_rc` directory, we highly suggest using the configuration files from the [mlvwmrc](https://github.com/morgant/mlvwmrc) project.

## DOCUMENTATION

We suggest reading the manual page (`man mlvwm`; English), but you may also find the original documentation helpful:

* README: [English](README), [日本語](README.jp)
* CONFIGURATION: [English](CONFIGURATION), [日本語](CONFIGURATION.jp)
* CHANGELOG: [English](CHANGELOG), [日本語](CHANGELOG.jp)
* Website: [English](http://www2u.biglobe.ne.jp/~y-miyata/mlvwm.html)

Note: the English documentation above was automatically generated from the Japanese documentation.

## CONTRIBUTING

Contributions are welcome and appreciated. Please read and follow the [CONTRIBUTING](CONTRIBUTING.md) guidelines.

## HISTORY

MLVWM was originally developed in 1997 by Takashi HASEGAWA, based on FVWM, while studying at Nagoya University. Active development proceeded through 2000. In 2020, Morgan Aldridge obtained permission to continue maintenance & development.

## LICENSE

This software is distributed as freeware as long as the original copyright remains in the source code and all documentation. Some files retain their original MIT license and one file is in the public domain.

Macintosh and MacOS are registered trademarks of Apple, Inc. (née Apple Computer, Inc.)
