# Linux on ARM Project
A side project started by [@MaxineToTheStars](1) that enables the use of Linux on aarch64 devices that originally shipped with Windows 10/11

## Overview
TBA

## Why?
While looking for a new laptop to buy, specifically one with long battery life and a solid performance mark, I stumbled across this lovely lady. The [Lenovo ThinkPad X13s](2). It included a 49.5 WHR battery, a Snapdragon 8cx Gen 3 Compute Platform SoC, up to 32GB of LPDDR4X RAM at 4266MT/s, and up to 1 TB of storage. The perfect mobile power house. I did some surfing before hand to see if... 

* The SoC is even supported in the Linux kernel
* It has been tested with "Just Works" distributions (Fedora, Ubuntu, Mint, etc)
* It was useable for daily use

All the forums I read and blog posts I saw all reported that *yes* Linux is suitable for this device it's not exactly the greatest. A bit bummed by the news I decided to wait till black friday (~1 month and some change of waiting) to see if the laptop will go down in price since it was and still is a tad too expensive for an aarch64 device. After seeing the price go down to the 1.3k mark (configured to my liking) I went ahead and bought the laptop. The day 1 experience of it was a bit of a struggle. After following the [Debian guide](3) and seeing the live environment have weird driver issues and fail to install I decided to do some more surfing and found [ironrobin's aarch64 Arch Linux iso made for the X13s](4). After flashing my USB with the new iso I was welcome by the warming embrace of Arch Linux running on kernel....5.19???? Yeah a tad old there however, WiFi did appear to be working. As of now I'm currently in the process of getting a nice Arch system up and running on the X13s. This organization will be my testing/documentation grounds on how to get this and many other aarch64 devices up and running with Linux. Enjoy your stay and **#EmbraceTheSuck**

## How's it going?
The same way x86_64 was with Linux in the 2000s... ok :+1:

[1]: https://github.com/MaxineToTheStars
[2]: https://www.lenovo.com/us/en/p/laptops/thinkpad/thinkpadx/thinkpad--x13s-(13-inch-snapdragon)/len101t0019
[3]: https://wiki.debian.org/InstallingDebianOn/Thinkpad/X13s
[4]: https://github.com/ironrobin/archiso-x13s