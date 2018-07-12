# openwrt-firmware
OpenWrt firmware for NETGEAR WNDR3800 with SS

## Firmware write

1. scp bin file to WNDR3800's `/tmp/` folder
2. run

    ```
    mtd -r write mingyue-20180227-openwrt-15.05.1-ar71xx-generic-wndr3800-squashfs-sysupgrade.bin firmware
    ```

## SS Install

With following order:

1. luci-app-ChinaDNS_1.3.1-1_all.ipk
2. luci-app-pdnsd_git-***-1_all.ipk
3. luci-i18n-pdnsd-zh-cn_git-***-1_all.ipk
4. Shadowsocks-libev-spec_3.1.0-2_***.ipk
5. luci-app-shadowsocks-spec_1.3.1-1_all.ipk

## Special thanks

1. [openwrt-ssr](https://github.com/rapistor/openwrt-ssr)
2. [Mingyue OpenWrt](https://www.myopenwrt.org/firmware-download)
