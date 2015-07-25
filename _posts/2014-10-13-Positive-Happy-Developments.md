---
layout: post
title: PhD – Positive, Happy, Developments
---

![headimg]({{ site.baseurl }}/images/RightOrWrong1921-225x300.png)
This post follows on directly from my [previous discussion](http://www.ecoevoblog.com/2014/10/06/phd-pretty-huge-disaster/) of my PhD going wrong. As a brief summary of the previous episode: I ran time consuming simulations that took me around 6 month to design and another 6 months to run. The simulation failed in the end because of a bug in some of the software I was using.

Therefore, I had to run them all over again!  That took me one day (at least to relaunch it, the simulations are actually still running). In this post I’d like to focus on the importance of starting to enforce good habits in using computers from the start of your PhD, whether you’re doing bioinformatics or field ecology.

Coding facilitates life. A lot. If I could only offer two tricks to remember they would be:

* **Writing function-based scripts:** which involves isolating functions (the bits that are actually doing stuff) from scripts in order to be able to reuse/modify them easily for further/new analysis.

* **Using version control:** which involves saving your work as you modify it and keeping a good track of the history so that when something goes wrong you know exactly which one was the last version that worked and which is the version that bugs.

There are loads of other good tips and many excellent blogs about how to start good coding habits (for example, [this one](http://nicercode.github.io/) or [that one](http://software-carpentry.org/blog/index.html)) so I am not going to develop the point here.

I’ll just try to make the point by using a philosophical-historical-dodgy example that convinced me to start coding. Coding is like using a printing press vs. a pencil to write a sentence: *I can write this sentence of 71 characters in approximately 16 seconds*. And that is, with a pencil. If I had to use a printing press, it would take me one second to input each character in the press (assuming I trained a lot) plus one seconds for actually pressing the sentence. So that’s 16 seconds with a pencil and 72 seconds using the printing press (4.5 times longer). If you’re not that old-school, you will use a computer to analyse your data and what often happens is that it will take you less time to do things "by hand" (e.g. modifying column names, removing rows with NAs, etc...) than to write fancy functions. So why bother?

Well it’s the same as using the printing press, if you just want to write the sentence once, then, sure, don’t bother, but if you need to write it 10 times? The writing would take 160 seconds and the printing takes only 81! Also you’re likely to make typos when copying the sentence with a pencil, but you won’t make any with the press!

And the same applies to your computer analysis. If you’re removing columns with NAs "by hand" it will probably take you less time than writing a function. But what if you have more tables? How can you be sure you didn’t miss any? And on the plus side, if you write function-based scripts, chances are that you already have a function that does remove the columns with NAs from a former analysis.

To follow up with [my previous post](http://www.ecoevoblog.com/2014/10/06/phd-pretty-huge-disaster/), applied, to me, this happened to be a salvation! Because I spent 6 months trying to apply bioinformatics good practice, it only took me one day to relaunch the whole analysis! I just had to change the name of the version of the software that was bugged and press enter...

The process of doing actual science (i.e. from coming up with an interesting idea to submitting the paper) is not a continuous and straight process and it can drastically change at every step and is more about trial and error than about succeeding straight off.

**Photo credit**: wikimedia commons

**[Original post](http://www.ecoevoblog.com/2014/10/13/phd-positive-happy-developments/)**


