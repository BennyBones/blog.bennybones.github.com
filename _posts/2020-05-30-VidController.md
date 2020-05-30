---
layout: post
title: Arduino based Video Controller
---

![_config.yml]({{ site.baseurl }}/images/20200530_VidCont0.jpg)
After coming back to Australian sooner than I would have liked due to the global pandemic, I have had a chance to set my desktop computer up again and look at doing some video work again. After re-installing Premiere Pro again I begain wondering how I could streamline things and I thought I could use a jog wheel to scroll through the footage. A custom controller with hot key buttons and macros would be great. I know there are some one the market but I am more of a DIY guy and building one would be more fun.

... So I set about designing something...

![_config.yml]({{ site.baseurl }}/images/20200530_VidCont1.jpg)

I have been looking long and hard at making an arduino based midi controller for one of my synthesisers and thought it would be too hard to change a few things and make one that works for all those features I use in Premiere: Copy, Paste, Scroll, Jump to point, etc.

My idea was to get a big jog wheel to scroll frame by frame, one of the most time consuming things I find is finding the right frame to cut the footage on. This will be a rotory encoder which also has a push funtion that will work as Play/Pause. I have seen this has been done a few times in youtube videos, which is where I got the idea. There will also be a cluster of 8 buttons which will be for transport controls and a second cluster for other important funtions such as cut, paste and the all important save key.

![_config.yml]({{ site.baseurl }}/images/20200530_VidCont2.jpg)
I designed a circuit board for this project as I am learning how to use KiCad. There are a few things I need to change in this design, such as using an Arduino Nano clone. After playing around with the code, the Nano will not work the way I want as you can not use the USB port as a USB keyboard connection. The Nano's ATmega328p doesn't work with the Keyboard.h library and throws up errors when compiling. I am going to need to use a Micro clone instead which uses the ATmega32u4 chip set. I will be loosing 6 pins but I can re-jigger my design to work.

I was also thinking of using both clusters of buttons as different button matrixes, but changing my design to having both clusters in the same matrix will save on pins and on the programming, maybe even the memory in the Micro. I am also going to add the click function of the encoder to make row 7 to the matrix. this gives me room to add 3 more buttons if I want. There is also 5 pins free for further expanding.

I've ordered a Micro clone from Aliexpress, now to play the waiting game. It gives me time to work on the code and design so when it does arrive, I can just drop it straight in.

All this, just to save some time with video editing, is it worth it? very debatable. Does it keep me busy during this pandemic? very much so.