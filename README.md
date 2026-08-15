# i5-4590-EFI-Hackintosh
A universal hackintosh EFI based on i5 4590 with H81 motherboards (No discrete graphics included)

This part of readme is English, for Chinese, scroll down.

I updated another release dedicated on Installing Mavericks to it. Please read the About-Mavericks.md for more close info.

这一部分的README是英语，中文版本请下滑阅读

我又更新了一个可以安装Mavericks的EFI，详细内容请阅读另一份About-Mavericks.md

## About this EFI

This EFI is based on H81 motherboard + i5 4590 (like said earlier)

I found a lot of H81/B85 boards with Haswell i5 EFIs on GitHub but most of them require a discrete graphic card, then I made this one

it's also available for ONDA H81C (That board's video output is dead and I can't fix it)

My Platform:

CPU: Intel Core i5 4590

Motherboard: FOXCONN H81 

GPU: Intel HD 4600 (Integrated)

RAM: 2 x 4G DDR3 1600

Storage: XSTAR SSD 120G

Sound Card: ALC662

Net Card: Realtek RTL8188EU (yes it's a USB dongle)

Chassis: You don't need to know

SMBIOS: Mac mini 2014 (i5-4260U) - This SMBIOS supports monterey without OCLP

## Caution

About drivers for USB dongle net cards, check out the links below:

`https://github.com/chris1111/WirelessAdapterCloverBigSur`

`https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter`

`https://github.com/chris1111/Wireless-USB-Big-Sur-Adapter`

Download the assets in releases section and install the required kexts by following the instructions in the installer.

## Direct Links for USB Dongle Drivers

For Mojave 10.14.6 and above using OpenCore, [click here to download](https://github.com/chris1111/Wireless-USB-Big-Sur-Adapter/releases/download/V18/Wireless.USB.Big.Sur.Adapter-V18.zip)

For Catalina 10.15.7 and below using Clover, [click here to download](https://github.com/chris1111/Wireless-USB-Adapter/files/10222459/Wireless.USB.Adapter-V17.zip)

If it fails to download, try using the 点这里下载 in the Chinese section

(Also these installers ONLY support macOS so make sure you download it when Windows is still there)

If you're using an onboard WiFi module or Intel/Broadcom card or whatever, make sure to add the essential kexts and enable them in config.plist

About sound card, mine is ALC662 and using layout-id 11

Make sure to confirm your sound card model and fill the correct layout ID in DeviceProperties. (ALC IDs are NOT universal)

## 中文 

本EFI基于H81主板+i5 4590 我发现GitHub上的大部分Haswell i5+H81/B85的黑苹果EFI都需要一块独显，便有了这个完全不需要独显的EFI

本EFI也兼容昂达H81C（那个主板视频输出炸了而且我不会修）

我的平台：

CPU: Intel Core i5 4590

主板: FOXCONN H81 

GPU: Intel HD 4600 （核显）

内存: 2 x 4G DDR3 1600

硬盘: XSTAR SSD 120G

声卡: ALC662

网卡: Realtek RTL8188EU (大概就是本🉑没钱买博通的网卡只能用pdd10块钱不到的USB网卡吧嗯对)

机箱: 你没必要知道。

SMBIOS仿冒型号: Mac mini 2014 (i5-4260U) - 这个smbios在不用OCLP的情况下兼容Monterey

## 注意

关于外置USB网卡的解决方案，可以去以下几个仓库下载专属驱动：

`https://github.com/chris1111/WirelessAdapterCloverBigSur`

`https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter`

`https://github.com/chris1111/Wireless-USB-Big-Sur-Adapter`

在releases下去下载最新的驱动，跟着安装器器的步骤去安装必要的kext

（顺便说一下那个安装器只支持macOS 记得在Windows还在时把它下载了）

如果你在用板载网卡或是Intel/博通网卡 记得添加合适的驱动并在config.plist里启用

## 国区福利

我知道有些人github下载慢的要死 所有我就把挂了镜像的下载直链放在这 一键下载

如果你在用Mojave 10.14.6及以上且是OpenCore引导 [点这里下载](https://gh-proxy.com/https://github.com/chris1111/Wireless-USB-Big-Sur-Adapter/releases/download/V18/Wireless.USB.Big.Sur.Adapter-V18.zip)

如果你在用Catalina 10.15.7及以下版本且是Clover引导 [点这里下载](https://gh-proxy.com/https://github.com/chris1111/Wireless-USB-Adapter-Clover/files/10222459/Wireless.USB.Adapter.Clover-V17.zip)

下载失败的话去英语那里的click here to download试试

关于声卡，我的型号是ALC662 layoud-id是11

记得确定你的声卡型号 然后去查阅你可以用什么layout-id 并在DeviceProperties下修改 （ALC ID不是通用的！）
