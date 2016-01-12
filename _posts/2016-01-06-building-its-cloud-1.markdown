---
layout: post
title:  "Building its cloud, part 1 : choosing the right server"
date:   2016-01-06 18:53:42 +0100
categories: server
---

# Building its cloud, part 1 : choosing the right server

Before starting to (bricoler) our cloud on a distant server, we wanna get one, right?

## Owning vs Renting a server
Buying a machine hosted by a private company should obviously be profitable on the long run. However at first it may be wise to rent it as to test it's performance or even compatibility for our use. I would add that in any case, a (wise) consumer should almost always avoid (engagement). You've understood, we're gonna rent a server.

## Physical server vs VPS
VPS stands for Virtual Private Server. It actually consists of a Virtual Machine (or sometimes a container) that run of top of a physical server. and on which the provider offers a root access (or quasi-root).

The price of VPS services has grealy shrinked during the last years. What have been considered as a cheap service from Digital Ocean is now way more expensive that Pulseheberg,..., or even OVH.

The virtual servers are more or less isolated one from the others, depending on the hypervisor (the technique used for virtualization) that is used.

## VPS : KVM vs OpenVZ
KVM is known for providing a better isolation between the VMs. Each VM got his own kernel that you can freely update without restrictions. You can stick with your Linux or even change for a NT kernel on which a Windows Server can be set up, it is up to you :)

OpenVZ is quite different as it behaves more like a container on some aspect. Every OpenVZ VMs share the **same** kernel (often a Linux 2.7) that obviously cannot be updated from a VM.
- The pros : it gathers the needs of a large number of VMs and allocate the physical ressources accordingly, which is far more efficient than limiting ressources to VMs in need on one side and having unused ressources on the other sides. It often results on a much lower price for the user.
- The cons : despite the impossibility to update your kernel, your performance are not guaranteed to be constant over time.

## My choice 
I personally wanted to use Docker on top of my VPS, a tool that (if you're not yet familiar with it) is totally awesome. The problem is, Docker must officially runs on top of a Linux 3.2 kernel, as it is explained here. "*Officially*" because there is some workarounds found that can be set up on the physical machine (on the provider side then) that are proposed for example by Digital Ocean.

I therefore considered this feature while doing a benchmark :

...

For performance comparison, I used the excellent serverbear script that make things such easy and share the results across the community. I also add that this awesome tool is much underused in France (please use it guys!) as I struggle to find KPIs for my providers. 
