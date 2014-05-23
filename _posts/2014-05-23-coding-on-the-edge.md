---
layout: post
title: The price you pay for coding on the edge
---

Every developer will sooner or later in her carreer make a concious choice what will compromise her weapons of the trade. Starting with your favorite hardware and OS and including your favorite programming language and tool chain a lot of decicions need to be made. And sometimes your decisions fire back at you.

## A decade worth of failures

I started my ongoing affair with my weapon of choice about 10 years ago, when I was introduced to the miracles and wonders of Zope. Back then it was in many aspects way ahead of its competition for example by introducing the idea of through-the-web, the so called TTW development. The Zope management interface - short ZMI - made it possible to actually build complex dynamic webpages and portals in a straight forward manner. This was both a joy to use for a newcomer like me but also served somehow as an entry drug to pick up programming.

As my code started to move to the filesystem and gradually away from the ZMI my focus ever so slowly shifted to the filesystem, *Nix system administration, Python packaging, deployment tools, monitoring, deployment, etcetera.

Nowadays I even tend to get obsessed with optimizing my local development setup to squeeze out every bit of productivity end effectivness I can. But I will elaborate on this part of
my daily chores eventually in a seperate post.

## Systems evolve and so do developers?

We use - amongst other things - the enterprise content management system Plone and try our best to keep all our running installs and projects as close to the latest stable version. This is a constant struggle that can only be undertaken with discipline and careful planing of the system architecture when it comes to deploying customer sites.

But after all these years I am getting bored with the status quo and usually we use a slightly newer setup and strive to keep ahead of time: the current stable development version has always been used in production during the last couple of years.

But sometimes your weapon of choice fails you. Newer development versions get installed automatically and interfere with your carefully crafted project setup.

Today we had to debug a suddently empty navigation box only to find out the the underlying template had changed. This update fixes a yearlong annoyance and finally uses an 'ul' for the navigation items listing. But nevertheless an unexpected update took place that demanded for a hotfix (this will probably be explained in a seperate post as well).

### So what?

Accidents will happen and no matter how careful you plan your setup and version pin all project resources there is a price you pay for living on the very edge. Upstream changes might affect your current project so always be prepared. As long as only our local development setup breaks all is not lost.

I am convinced that the price we pay is worth the benefits to be had. We have things mostly up to date and under our control. The time spend for hotfixes like todays chores are an annoyance but nothing compared to the hours of development and upgrade work we spare by doing these small tests and incremental updates in our everyday work.

Optimize a little bit every day and the benefits will outweight the small problems that sometimes slow down development.
