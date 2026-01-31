---
layout: download-page
title: Download for openSUSE
permalink: /download/opensuse/
class: download

distro_name: openSUSE
distro_icon: opensuse.svg
distro_accent: '115,186,37'
order: 3

view_on_openrazer: https://openrazer.github.io/#opensuse
---

{:.warning}
> Native packages are **not available for Leap 15.6** because some required software (dependencies) are not available. Consider the [Flatpak](/download/flatpak) version for Leap 15.6 (and newer).

To add the repository, open the Terminal:

### Tumbleweed

```shell
sudo zypper addrepo https://download.opensuse.org/repositories/hardware:/razer/openSUSE_Tumbleweed/hardware:razer.repo
sudo zypper refresh
sudo zypper install polychromatic
```

### Leap 15.5

```shell
sudo zypper addrepo https://download.opensuse.org/repositories/hardware:/razer/openSUSE_Leap_15.5/hardware:razer.repo
sudo zypper refresh
sudo zypper install polychromatic
```

## OpenRazer

Polychromatic shares the repository with OpenRazer. It will be automatically installed when installing this software.

You'll need to add your user to the `plugdev` group. Reboot afterwards for changes to take effect.

```shell
sudo gpasswd -a $USER plugdev
```
