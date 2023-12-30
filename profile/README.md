# Linux on ARM Project
A side project started by [@MaxineToTheStars][1]. Enables the use of Linux on AArch64 devices that originally shipped with Windows 10/11.

## Overview
> [LinuxOnARM/linux][overview-1] - A fork of the Torvalds Kernel with included patches for AArch64 systems.
> [LinuxOnARM/archiso-aarch64][overview-2] - A fork of the Arch Linux [archiso][overview-2-1] repository made for AArch64 systems.
> [LinuxOnARM/alarm-pkgbuilds][overview-3] - A custom automated building and packaging system for Arch Linux AArch64 devices. The GitHub repository also acts as a package repository.

## Why?
While looking for a new laptop to buy, specifically one with an "all-day battery" and solid performance number, I stumbled across this lovely lady. The [Lenovo ThinkPad X13s (Gen 1)][2]. It includes a 49.5 WHR battery, a Snapdragon 8cx Gen 3 Compute Platform SoC, up to 32GB of LPDDR4X RAM at 4266MT/s, and up to 1 TB of storage. The **perfect** mobile power house. Just one minor issue, it comes preloaded with Windows 11 on ARM. Now if this was an x86_64 laptop this wouldn't be such a hassle. Just boot up your favorite Linux distribution, in my case Arch Linux, and enjoy your new machine. However, this is an AArch64 powered laptop so a couple things had to be confirmed first...

* Is the SoC is supported in the Linux kernel?
* Has it been tested with "Just Works" distributions? (Fedora, Ubuntu, Linux Mint, etc)
* Driver support?
* Is it even suitable for Linux?

All the forum and blog posts I read all reported that *yes*, Linux can indeed run on this machine however, it won't exactly be the greatest experience. Some even describe it as using a x86_64 machine with Linux in the 2000s. After buying and unboxing the laptop I got my trusty USB stick pre-loaded with Debian 12 for ARM and booted it up. I followed the [Debian guide][3] for installing Linux on the ThinkPad X13s but to no avail. Weird driver issues and DBT files missing made the install process a pain. Bummed out by the fact I couldn't get Debian to work I decided to try out [ironrobin's AArch64 Arch Linux ISO][4]. This ISO was built/generated for the X13s so it's worth a try. After flashing the USB and rebooting my laptop I was greeted to the Arch Linux live environment....I'm sorry does that say Kernel version 5.19???. After that whole ordeal I decided to create a GitHub organization that will serve as a development, documentation, and testing ground on how to get this and many other AArch64 devices up and running with Linux. I hope you enjoy your stay and remember, **#EmbraceTheSuck**.

## How's it going?
The same way x86_64 was with Linux in the 2000s... ok :+1:

[1]: https://github.com/MaxineToTheStars
[2]: https://www.lenovo.com/us/en/p/laptops/thinkpad/thinkpadx/thinkpad--x13s-(13-inch-snapdragon)/len101t0019
[3]: https://wiki.debian.org/InstallingDebianOn/Thinkpad/X13s
[4]: https://github.com/ironrobin/archiso-x13s

[overview-1]: https://github.com/LinuxOnARM/linux
[overview-2]: https://github.com/LinuxOnARM/archiso-aarch64
[overview-2-1]: https://github.com/archlinux/archiso
[overview-3]: https://github.com/LinuxOnARM/alarm-pkgbuilds