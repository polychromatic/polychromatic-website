---
layout: download-page
title: Download for Gentoo
permalink: /download/gentoo/
distro: gentoo
distro_name: Gentoo
distro_accent: '158,149,247'
class: download

backends:
    openrazer: https://openrazer.github.io/#gentoo
---

These packages are maintained by [vifino] in the [vifino/vifino-overlay] repository.

```shell
eselect repository enable vifino-overlay
emaint sync -r vifino-overlay
emerge app-misc/polychromatic
```

For packaging or dependency problems, please [raise the issue] in their repository.

[vifino]: https://github.com/vifino/
[vifino/vifino-overlay]: https://github.com/vifino/vifino-overlay/tree/master/app-misc/polychromatic/
[raise the issue]: https://github.com/vifino/vifino-overlay/issues
