# openwrt-firmware
OpenWrt firmware for NETGEAR WNDR3800 with SS

## Mingyue firmware
### 1. Firmware write

1. scp bin file to WNDR3800's `/tmp/` folder
2. run

    ```
    mtd -r write mingyue-20180227-openwrt-15.05.1-ar71xx-generic-wndr3800-squashfs-sysupgrade.bin firmware
    ```

### 2. SS Install

With following order:

1. luci-app-ChinaDNS_1.3.1-1_all.ipk
2. luci-app-pdnsd_git-***-1_all.ipk
3. luci-i18n-pdnsd-zh-cn_git-***-1_all.ipk
4. Shadowsocks-libev-spec_3.1.0-2_***.ipk
5. luci-app-shadowsocks-spec_1.3.1-1_all.ipk

## Lean OpenWrt

This firmware is almost perfect for WNDR3800, and check [this for details](http://www.right.com.cn/forum/forum.php?mod=viewthread&tid=255640&highlight=3800).

And the firmware file is `R7.61-180410-generic-wndr3800-squashfs-sysupgrade.bin`.

## Special thanks

1. [openwrt-ssr](https://github.com/rapistor/openwrt-ssr)
2. [Mingyue OpenWrt](https://www.myopenwrt.org/firmware-download)
3. [Lean OpenWrt](http://www.right.com.cn/forum/forum.php?mod=viewthread&tid=255640&highlight=3800)
