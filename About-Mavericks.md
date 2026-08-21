# About Mavericks

这部分的About Mavericks是英语，中文请下滑阅读。

## Prologue

I honestly don't know why I want this PC to run a Mavericks (cause skeuomorphism is cool, I think?) on it all of a sudden

Then I made some tweaks (and it took me hours to debug fahhhhhh) and it successfully booted! That was unexpected btw

So I decided to upload another package for people who want some neat skeuomorphism design and old-school Apple feeling, even if Mavericks is basically cripped in nowaday's software environment

WARNING: It's still work in process and it's not out-of-the-box. Take some time to debug it if you can.

## Precautions

If you still don't have a Mavericks image, you can download it in my Releases tab, unzip it and simply put it in the same directory as the EFI. (However I still strongly recommend using a full installer, the reason is below)

If you want Monterey (macOS 12), DO NOT USE THIS EFI. Download the another one in Releases tab.

Also, prepare your Apple ID (Better be a backup one) if you're using an online recovery image. I have no idea why Apple needs your account just for reinstalling the system but they just did (Apple sucks)

Most kexts work in Mavericks but some don't. The exceptions are USB mapping kexts (USBMap & UTBDefault) and RealtekRTL8111. 

I downgraded the RealtekRTL8111 to a older version, and it seems compatible.

Next is the USB mapping problems. And because there's no USB port limit on Mavericks, and my newer Catalina seems also don't need a USB mapping kext(s), so, case closed.

For now, this EFI can boot to recovery environment successfully. If anything is not working (Graphics, Sounds, or whatever) please add an issue and let me know.

# 中文

## 前言

我估计是脑子抽抽了，不知道为啥突然想让这台电脑跑个Mavericks（也许拟物化更有感觉？）

之后我在之前的EFI上做了点调整（牛魔的花了我几个小时调试wdnmd）然后还真启动了！我还真没想到。

所以为了喜欢拟物化和大果公司老设计的人，我就想再上传一个EFI整合包，就算Mavericks在当今的软件生态里是个十足的瘸子。（体验在先嘛）

注意：这个EFI不是开箱即用，找个时间好好调试一下也不是不行。

## 注意事项

如果你依旧没有Mavericks的镜像，你可以在Releases下下载在线恢复镜像com.apple.recovery.boot.zip, 解压后放到和EFI一样的目录就好（但是我依旧强烈推荐用离线镜像，大概5GB，原因在下面）

如果你要用Monterey (macOS 12)，### 不要用 ### 这个整合包！去Releases栏下载另一个。

并且如果你要用在线恢复（Mavericks），请准备好你的Apple ID（最好是备用）。鬼知道为什么苹果就连重安系统都要账号，但苹果确实这么做了（大果四凤了）

大部分的kext依旧在Mavericks工作，但有几个例外。分别是给USB映射用的kext (USBMap & UTBDefault) 和 RealtekRTL8111. 

我给RealtekRTL8111降了个级，貌似可以用。

接着就是USB映射的问题。因为Mavericks并没有USB端口限制，我目前在用的Catalina没了USB映射的kext（好像）也可以正常用，那就结案了。

目前这份EFI可以成功进入恢复环境。如果有东西用不了，请在issue里点拨一下。
