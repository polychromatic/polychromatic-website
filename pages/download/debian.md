---
layout: download-page
title: Download for Debian
permalink: /download/debian/
class: download

distro_name: Debian
distro_icon: debian.svg
distro_accent: '215,7,81'
order: 1
---

{:.warning}
> **Debian 13 and later no longer accept the SHA-1 signing key as of February 2026.**
>
> Check back here later this month after we build a new repository.
> The one hosted on Launchpad will continue to work until February 2026.

To add the repository and install, open the Terminal:

```shell
echo "deb [signed-by=/usr/share/keyrings/polychromatic.gpg] http://ppa.launchpad.net/polychromatic/stable/ubuntu noble main" | sudo tee /etc/apt/sources.list.d/polychromatic.list
curl -fsSL 'https://keyserver.ubuntu.com/pks/lookup?op=get&search=0xc0d54c34d00160459588000e96b9cd7c22e2c8c5' | sudo gpg --dearmour -o /usr/share/keyrings/polychromatic.gpg

sudo apt-get update

sudo apt install polychromatic
```

### OpenRazer

OpenRazer is in the [official Debian repositories], but it can be a few versions behind.
If you need to use a device, feature or fix that was [released in a newer version], add [OpenRazer's repository for Debian].

You'll need to add your user to the `plugdev` group. Reboot afterwards for changes to take effect.

```shell
sudo gpasswd -a $USER plugdev
```

[official Debian repositories]: https://packages.debian.org/search?keywords=openrazer
[released in a newer version]: https://github.com/openrazer/openrazer/releases
[OpenRazer's repository for Debian]: https://software.opensuse.org/download.html?project=hardware%3Arazer&package=openrazer-meta


### About the repository

Launchpad acts as the repository host for this package archive.
Packages and dependencies are compatible and tested between Debian and Ubuntu.

The series are mapped as follows:

* `jammy` for Debian 11 "Bullseye" (Qt 5)
* `noble` for Debian 12 "Bookworm" (Qt 6)
* `noble` for Debian 13 "Bookworm" (Qt 6)
