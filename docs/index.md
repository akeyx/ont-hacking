---
title: Replacing Nokia ONT with SFP+ Leox LXT-010S-H
parent: Home nav_order: 1
has_children: true
---

# Replacing Nokia ONT with SFP+ Leox LXT-010S-H

This page documents how to replace ISP issued Nokia ONT (eg. G-010G-Q or G-010G-R) with your own. Here I'll use Leox [LXT-010S-H|https://www.leolabs.pl/ont-leox-lxt-010s-h.html].

# But Why ?

Because:
- I want to
- I can
- I don't want to have yet another device in front of my router
- I want to have full control over my network
- etc.

# What's required

- Visual access to the back of the original ONT
- A Linux workstation (because it's: easier, better, nicer, free, etc. )
- Tools: 
 - telnet
 - netcat/nc
 - binwalk
 - strings
 - grep
- A router that can take in SFP+ modules eg. a Mikrotik HEXS or RB0009 or similar router.

# Preface

There's already a fair number of blog posts etc. documenting how to do this sort of thing but pretty much all of them go through the case of ONT being Huawei and require almost zero config or using some basic settings which don't really work with Nokia ONTs/ONUs so here I'm documenting the full process of replacing such ISP issued device with your own focusing on most important bits like obtaining the right firmware version etc.
