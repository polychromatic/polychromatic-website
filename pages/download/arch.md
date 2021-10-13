---
layout: download-page
title: Download for Arch
permalink: /download/arch/
distro: arch
distro_name: Arch Linux
distro_accent: '23,147,209'
class: download

backends:
    openrazer: https://aur.archlinux.org/packages/openrazer-meta/
---

{% capture stable %}

Polychromatic is [available from the AUR](https://aur.archlinux.org/packages/polychromatic/).
For example, using an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers#Comparison_tables):

```shell
yay -S polychromatic
```

{% endcapture %}

{% capture edge %}

Polychromatic is [available from the AUR](https://aur.archlinux.org/packages/polychromatic-git/).
For example, using an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers#Comparison_tables):

```shell
yay -S polychromatic-git
```

Depending on the AUR helper, you may need to manually update/rebuild this
package if you wish to get the latest changes.

{% endcapture %}

{% include partials/download-tabs.html
    stable=stable
    edge=edge
%}
