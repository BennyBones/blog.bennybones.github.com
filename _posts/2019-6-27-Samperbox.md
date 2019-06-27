---
layout: post
title: SamplerBox
---

This is my build of a SamplerBox.

![_config.yml]({{ site.baseurl }}/images/20190627_Sampler1.jpg)
![_config.yml]({{ site.baseurl }}/images/20190627_Sampler2.jpg)

The main reason I wanted to build a little sample player is that I needed some way of playing samples live on stage without having to buy a $300+ sample player and without having to rely on using a laptop. I have been using many different laptops and setups over the past 3 years and I find them to be very unreliable when on stage. My initial idea was to sample all the sounds I use from my hardware rack synths, an aging Korg Wavestation SR and a Korg MS2000R, and play them with my midi controller along with the triggerable samples I use during our set. Having something light weight and easy to set up was key to my plans, as well as cheap and DIY.

I started building a Raspberry Pi sample player, know as a [SamplerBox](http://www.samplerbox.org), about a year ago. I started with a Pi3b which was running a [modified version](https://samplerbox.readthedocs.io/en/latest) of the original SamplerBox iso and designed a 3d printable case for it. This case houses the Pi, the 2x18 LCD screen, the button board, and all the usb attachments (ie, sound card, thumb drive and midi-to-usb adapter). It was designed in Tinkercab and is only basic, but it was enough for me to store everything I needed at the time with plenty of room for further modifications.

After accidentally destroying the pi with a rogue drill bit I went up to a Pi3b+. The software I had for the B wouldn't run on the B+ as the architecture was different as the B+ is a 64-bit ARMS chip rather than a 32-bit like its predecessor so I had to change to [another veriaton](http://homspace.xs4all.nl/homspace/samplerbox/index.html) of the original iso, this time by Hans. Although there are a few bugs still in this version, Hans is working hard at getting everything working right.

There are some differences between the two builds, the menu systems and the way they are controlled, but the overall functionality is the same.

Tonight will be my first 'live' test of the SamplerBox in the jam room ahead of a gig this weekend.
