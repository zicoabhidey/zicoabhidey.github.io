---
layout: post
title:  "Guide for buying Wireless lan adapter for Ubuntu in 2020"
date:   2020-04-19 05:34:19 +0800
categories: Default
tags: Ubuntu Anaconda
comments: 1
---
Not all the oems write driver their own wireless lan adapter. You can found plathera of wlan nwtwork adapter available online from oems who does not provide proper support or instruction for setting up in linux.

The best way to choose a Wireless lan adapter based on its chipset inside. Then you can look for drivers online (in many cases available in github). I myself own a wlan adapter with rtl8812au chipset and will recommend you to to buy one.

Aircrack-ng has a repository available in github for rtl8812au driver. https://github.com/aircrack-ng/rtl8812au

Here is how you can set it up by running the following commands in the terminal
```bash
git clone https://github.com/aircrack-ng/rtl8812au.git
cd rtl8812au
sudo ./dkms-install.sh
sudo modprobe 88XXau
```

If you are not so sure which one to buy or do not want to research before buying, gentoo linux has [a list of rtl8812au devices](https://wiki.gentoo.org/wiki/AC1200_Wireless_Adapters)
