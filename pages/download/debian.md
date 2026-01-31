---
layout: download-page
title: Download for Debian
permalink: /download/debian/
class: download

distro_name: Debian
distro_icon: debian.svg
distro_accent: '215,7,81'
order: 1

view_on_openrazer: https://openrazer.github.io/#debian
---

{:.warning}
> **Repository updated for Debian 13 onwards**
>
> Debian 13 "Trixie" no longer accepts the SHA-1 signing key as of February 2026.
> We've created a new repository for Debian to replace the Launchpad one.
>
> If you use Debian 12 "Bookworm" or earlier, the Launchpad repository will continue to work.

To add the repository and install, open the Terminal:

```shell
curl -fsSL 'https://debian.polychromatic.app/key.asc' | sudo gpg --dearmour -o /usr/share/keyrings/polychromatic.gpg

source /etc/os-release
echo "deb [signed-by=/usr/share/keyrings/polychromatic.gpg] https://debian.polychromatic.app $VERSION_CODENAME main" | sudo tee /etc/apt/sources.list.d/polychromatic.list

sudo apt-get update

sudo apt install polychromatic
```

### OpenRazer

OpenRazer is in the [official Debian repositories], but it could be a few versions behind.

```shell
sudo apt install openrazer-meta
```

You'll need to add your user to the `plugdev` group.

```shell
sudo gpasswd -a $USER plugdev
```

Reboot afterwards for changes to take effect.

For the [latest device support and fixes], we'd recommend using OpenRazer's own repository.

[official Debian repositories]: https://packages.debian.org/search?keywords=openrazer
[latest device support and fixes]: https://github.com/openrazer/openrazer/releases
