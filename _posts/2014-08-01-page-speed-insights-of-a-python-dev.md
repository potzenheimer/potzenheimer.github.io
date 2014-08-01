---
layout: post
title: How page speed is the most responsive part in RWD
---

Over the last couple of days several smarter people than me have posted their ideas on making sites load with maximum speed and elaborated on the suble differences in user experience when facing slow loading pages on a crappy mobile network.

Basically it all boils down to the simple fact that optimizing a website for mobile usage the site must load as fast as possible in order to be usable on a shaky EDGE network. Webdesigners and developers need to respond to the rising trend of mobile internet usage by building sites that focus on speed from the early stages of design and concept.

## A primer and a failure

These days I mostly get my incentives from [Smashing Magazine](http://smashingmagazine.com) and the connected editor-in-chief curated Twitter channel `@smashingmag`. Recently the discussions have been revolving around the [critical loading path](http://www.feedthebot.com/pagespeed/prioritize-visible-content.html), technics for ["breaking news at 1000ms"](https://twitter.com/smashingmag/status/494949979820417024) at the Guardian or how large and well known sites [organize frontend architecture](https://twitter.com/smashingmag/status/495024899648278528).

Therefore the last days have been glorious and filled with exiting reads that made me suck in the information and learn my share from how development work is done by the big guys in the business.

But what a disappointment to find the latest issue of [Website Boosting Magazine](http://www.websiteboosting.com/) and skim through an article focusing on on-page search engine optimization and finding a rather high number of advice that is just plain wrong. Coming from [optimising for 60fps everywhere](https://engineering.gosquared.com/optimising-60fps-everywhere-in-javascript) I could not believe that the articles author was actually trying to tell me to do the exact opposite than what I had learned earlier today.

## But what is this fuss all about?

Well in order to be fair it has to be stated that the Website Boosting article was written by a marketing and communications professional and that the best web development professionals of the trade might probably be years ahead in knowledge.

But reading that one should put your CSS and Javascript code into linked external files to speed up one's site for search engine optimization while others promote inlining the critical CSS/JS to speed up things is quite a stretch.

The browser needs to download and parse any HTML, CSS and JavaScript before all pixels can be written to the screen as required. And it only has *16ms* to accomplish this - not exactly what you would call a hell lot of time.

And while we all promote to use the latest and greatest HTML5/CSS3  - whatever you want to call all the fancy - since we do not have to support broken browsers any more (I am looking at you IE), we tend to develop a sane and straight forward coding style.

Per HTML5 spec, typically there is no need to specify a type when including CSS and JavaScript files as text/css and text/javascript are their respective defaults:

    <!-- JavaScript -->
    <script src="application.js"></script>


I find it rather odd, to find code examples like the following in a magazine **fresh out of the press**

    <script language="JavaScript" type="text/javascript" src="main.js"></script>


This hurts my eyes and makes me sad. The good and the bad all in one day - and these are just the most obvious examples, why I believe that a huge part of the web business already has lost the connection to its most valuable resource - the actual visitors of their sites, services and apps.


