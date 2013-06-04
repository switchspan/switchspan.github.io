---
layout: post
title: Raspberry Pi...Finally!
date: 2013-01-14 09:30
comments: true
categories: [hardware]
---
{% img right /images/IMG_1420.jpg 244 184 Pi size comparison %}
Christmas really did come early last year: I finally received my [Raspberry Pi](http://www.raspberrypi.org/) model B direct from the UK!  The Raspberry Pi has been so popular that there has been quite a few delays in production and delivery of these tasty little computers -- and at $25 a piece they are economical and tasty!
<!-- more -->
## The Un-Boxing

{% img left /images/IMG_1413.jpg 244 184 Unpacking the Pi %}
I ordered my Raspberry Pi from [RS Online](http://uk.rs-online.com/) around August and received it the week of November 26th (2012). The demand for these little computers has been tremendous and there are only a few authorized direct vendors in the UK (you can visit the [Raspberry Pi site](http://www.raspberrypi.org/) to find the vendors).     

My entire order consisted of the following:

* Raspberry Pi model B  
* RS Electronics protective case  
* 4 GB SD Card Pre-loaded with [Raspbian](http://www.raspbian.org/) ([Debian](http://www.debian.org/) "Wheezy" based Linux)  
* [RCA Stereo cables](http://en.wikipedia.org/wiki/RCA_connector)  


{% img right /images/IMG_1496.jpg 244 184 Arduino and Pi %}

What I initially noticed when I opened the packaging to my new toy was the size of the Raspberry Pi. I have an [Arduino](http://www.arduino.cc/) Uno and the Raspberry is nearly as small as the Uno.  After unboxing and taking pictures of all of the pieces, I worked on getting the Raspberry Pi into the protective case made by RS. This required a small amount of ‘gingerly’ trying to push the Raspberry Pi into place without breaking it or the case, but after a few minutes I figured out the easiest way to get it into and out of the case. 
## Initial Setup

{% img left /images/IMG_1438.jpg 244 184 Keyboard and mouse %}

To connect the Raspberry Pi, you will need a USB keyboard, mouse, a Type B USB Plug (the size that most printers use), A [USB AC Wall Adapter/Charger](https://www.sparkfun.com/products/11456) and either an [HDMI](http://en.wikipedia.org/wiki/HDMI) connector or [RCA](http://en.wikipedia.org/wiki/RCA_connector) cable. 
If you want sound you might want to get a [stereo](http://en.wikipedia.org/wiki/Stereo_jack) to [RCA](http://en.wikipedia.org/wiki/RCA_connector) jack adaptor.  

I started with plugging in the keyboard and most first, as it did not require power.

My next activity was to plug the Pi into my TV via the RCA jack. 

{% img right /images/IMG_1426.jpg 244 184 Hardcase and memory card %}
Always remember this with the RCA jacks: Yellow jacks are typically video, and your Red and White jacks are for left and right audio (stereo). On the Raspberry Pi, the video RCA jack is the same size on both ends, but the audio RCA is two regular size jacks which pair down into a small MP3 headphone size jack that plugs into the Pi. 
You can see the RCA video plug in the pic below and the RCA audio plug is the small black plug next to it. 
To start the Pi up, I plugged the USB charger into the wall and the USB Type B connector into the back of the Raspberry Pi. 

The Raspbian menu lets you initially configure a lot of items which you will be potentially searching for after the setup -- such as making it boot directly into X windows.
If you have kids using it, making it boot into X windows is a **MUST**.  **Note:** Once you set your defaults from the first boot up, you will not see the configuration page again (I would have a pic of this had I known!).
*You will have to ‘role up the sleeves’ and configure some Unix/Linux configuration files to make any changes after the initial setup.* 

## Boot Up

The pic you can see below is the first boot up. 

{% img left /images/IMG_1435.jpg 244 184 First boot up %}
The boot up screen shows some typical Linux boot-up kernel ring buffer messages. 
The Raspberry Pi's boot up was rather speedy and took only a few seconds
- the benefit of booting off of a flash drive. 
The Raspberry Pi is capable of detecting on boot whether you have the RCA jack plugged in or the HDMI cable plugged in. 
I recommend HDMI if you have a flat screen as it seems to be abled to handle the screen resolutions better than the RCA jack. &nbsp; 

## Pi Desktop

{%img right /images/IMG_1462.jpg 244 184 Raspberry Pi desktop %}

The Raspberry Pi logo is prominent on a rather clean desktop look. All of the main items such as the [IDLE](http://docs.python.org/2/library/idle.html), [Scratch](http://scratch.mit.edu/) and Python Games.

My sons enjoyed playing the “[Squirrel Game](http://pygame.org/project-Squirrel+Eat+Squirrel-1853-3764.html)” which consists of trying to eat smaller squirrels to make your squirrel bigger. 
They kept at it until they won the game.  
My older son also played with scratch quite a bit – but it kept locking up, which I believe might be due to the under-powered [USB](http://en.wikipedia.org/wiki/Universal_Serial_Bus) hub I was using. 
{% img left /images/IMG_1464.jpg 244 184 The Squirrel Game %}
You really have to make sure you have a powered one, as the Pi can only supply so much power for the [2 USB ports](http://en.wikipedia.org/wiki/Universal_Serial_Bus) that it has.
Once you have a keyboard and mouse plugged in there is not much room for more. 
I used a USB hub to give me a little more ‘reach’ with my keyboard and mouse, so they didn’t have to be directly in front of the TV. 
The moral here: Make sure you have enough power for the USB bus – a steady 5 volts DC. Also: You will want a decent USB hub if you want to use more than the 2 USB Type A Plugs that are on the front of the Raspberry Pi.
   
## Game Over

{% img center /images/IMG_1445.jpg 244 184 Game Over %}
So, it is ‘Game Over’ for this post on the Raspberry Pi. I will continue to tinker with it and hopefully have some more items to report.
