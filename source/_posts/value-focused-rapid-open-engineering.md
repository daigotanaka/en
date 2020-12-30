---
title: Value-focused, rapid, open engineering
date: 2014-05-09 00:00:00
tags:
---

![Voice operating wearable computer](http://farm6.staticflickr.com/5548/9330154869_72b8d882b2_b.jpg)

Since last July, I have been working on making a voice operating
[mini-computer](http://daigolab.org/chattypi/) that is meant to be carried with
me so I can breathe information in and out while I am on the move. For example,
I can search for a short answer simply saying the question: "What is the
weather in Mountain View today?" I ask this question to the mini-computer every
morning as I get ready to go out. It also reads out the message to my ear when
someone sends me an instant message. It actually learns from the inbound
texts to enhance the voice recognition capability.

The quality of this computer is far from the level to be called a commercial
product. But it is something I can develop little by little based on my own
desire and imagination. It is very satisfying to use what I made just as I
enjoy eating what I have cooked.

As I use what I create, I also find things that I want to improve. Then I rip
the old code, and quickly re-design and re-write the code. I think this
computer and other things I create increase their value little by little this
way.

Although they are not commercial products, I take a value-driven approach. I
want to be benefited by what I code as fast as possible. Or at least I want to
come up with a prototype of the idea very quickly so I can learn if it changes
my life, and possibly of others.

To build quickly, I am shameless about using other people's work. Probably, the
most technologically complicated part of the voice operating computer project
is voice recognition.  I did not develop this. I first recorded audio, and used
Google's speech-to-text web service. But Google recently made a serious limit
on the audio file size that can be sent to the server, and it became impossible
to parse voice.  So I compiled CMU Sphinx [^cmusphinx] on Raspberry Pi
[^raspberrypi] and running voice recognition on the mini-computer. Voice
recognition requires to build a good language model for a good accuracy. So, I
am using the text coming in through the instant messenger and search results as
the example sentences to build such model.

Overall, my personal projects typically have these three characteristics:

1. Focus on delivering value. Something I can try using right away.
2. Avoid re-inventing the wheel. Use other people's work and focus on designing
the applications.
3. In return, [share](http://www.daigotanaka.org/creative-commons-open-source/)
what I create to the world.

This project has been a lot of fun, and I see bigger potential. I am going to
integrate this voice operating computer with
[my server code](http://www.daigotanaka.org/website-source-code/) to log the
information around my life, and feed myself with useful information based on
data analysis. It could also be integrated with
[a robot](http://daigolab.org/roomba-telepresence-robot/), I suppose.

[^cmusphinx]: [CMU Sphinx - Speech Recognition Toolkit](http://cmusphinx.sourceforge.net/)
[^raspberrypi]: [Raspberry Pi](http://www.raspberrypi.org/)

