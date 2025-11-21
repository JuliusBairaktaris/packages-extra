# Extra Packages

Extra OpenWrt + LuCI packages, focused on NSS builds for IPQ807x/IPQ60xx platforms.

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-IPQ807x%20%7C%20IPQ60xx-007ACC.svg)](https://www.qualcomm.com/)

---

## Overview

A small collection of utility and LuCI packages tailored for [NSS builds of OpenWrt](https://github.com/qosmio/openwrt-ipq). Packages here aim to be minimal (and buggy) but mostly compatible with NSS-enabled firmwares.

## Packages

| Package | Description |
|---|---|
| [luci-mod-status-nss](modules/luci-mod-status-nss) | LuCI status module that provides real-time temperatures for WiFi radios, CPU cores, and NSS components. |

## Installation (feed-level)

Add this repository to your OpenWrt feeds, update, and build as usual:

```bash
# add feed (example)
echo "src-git qosmio https://github.com/qosmio/packages-extra" >> feeds.conf.default

# update and install
./scripts/feeds update qosmio
./scripts/feeds install -a -p qosmio

# configure and build
make menuconfig
```

<div align="center">

If you find this useful, consider supporting the project:

[![Donate with PayPal](https://github.com/qosmio/openwrt-ipq/raw/main-nss/paypal.png)](https://www.paypal.com/donate?business=3V3H2SZFY7DNQ&item_name=Maintaining+NSS+fork+of+OpenWRT+and+NSS+packages.)
<a href="https://cash.app/$austinzk">
  <img src="https://github.com/qosmio/openwrt-ipq/raw/main-nss/cashapp.png" alt="Cashapp" width="150px"/>
</a>

</div>
