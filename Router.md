# Router

## TP-Link TL-WR741N/ND v4

CPU Atheros AR9330 rev 1
内存 64MB DDR
闪存 Winbond W25Q64 @ 20MHz (8MB)
以太网 Atheros AR8216 (built-in) rev 2
系统频率 CPU: 400MHz, DDR: 400MHz, AHB: 200MHz, Ref: 25MHz
编译日期 2014-11-23 01:29:25 +08:00

TL-WR741ND v4.x
Version 4.x has changed to use the AR9331 SoC, and is supported by the trunk version.
Probably the hardware of all v4.x versions is identical.

After installation of r31249 + LuCI, 604KB flash are free for additional packages.

/proc/cpuinfo

  system type             : Atheros AR9330 rev 1
  machine                 : TP-LINK TL-WR741ND v4
  processor               : 0
  cpu model               : MIPS 24Kc V7.4
  BogoMIPS                : 265.42
  wait instruction        : yes
  microsecond timers      : yes
  tlb_entries             : 16
  extra interrupt vector  : yes
  hardware watchpoint     : yes, count: 4, address/irw mask: [0x0000, 0x0ff8, 0x0ff8, 0x0ff8]
  ASEs implemented        : mips16
  shadow register sets    : 1
  kscratch registers      : 0
  core                    : 0
  VCED exceptions         : not available
  VCEI exceptions         : not available



opkg update
opkg install luci-i18n-base-zh-cn
http://openwrt-dist.sourceforge.net/auto_install_lede.sh
luci-app-shadowsocks_1.9.0-1_all.ipk
ShadowVPN_0.2.0-1_mips_24kc.ipk
luci-app-shadowvpn_1.6.1-1_all.ipk



wget http://openwrt-dist.sourceforge.net/auto_install_lede.sh -O /tmp/auto_install_lede.sh
chmod +x /tmp/auto_install_lede.sh
/tmp/auto_install_lede.sh  # 执行此步骤时候按照提示，选择安装shadowsocks,chinadns以及dns-forwarder
opkg install ip-full iptables-mod-tproxy




CPU Atheros AR7161 rev 2
内存 128MB SDRAM
闪存 Macronix MX25L12805D @ 28MHz (16MB)
以太网 Realtek RTL8366S/SR ver 1
系统频率 CPU: 680MHz, DDR: 340MHz, AHB: 170MHz, Ref: 40MHz
编译日期 2014-10-07 21:11:07 +08:00