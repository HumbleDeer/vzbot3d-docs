---
layout: default
title: Watercooling
parent: Vz-Other
has_toc: true
has_children: true
---

# Watercooling your VzBot

This document will go over the steps and materials required to watercool any components of your VzBot that may benefit from watercooling.  
You may also watercool things that don't require watercooling; it looks cool, we admit that!

The following components of your VzBot can be easily watercooled with thermal benefits:

1. [Goliath] hotend
2. [Vz-HextrudORT]
3. Stepper motors
4. Stepper motor drivers

## Benefits

The benefits of watercooling your VzBot come from a variety of aspects about your VzBot and its thermal performance. The most important parts to cool are the stepper motors driving the A/B axes, and the printhead components.

When the [Vz-hextrudORT] and [Vz-Printhead] are made of aluminium, they both conduct heat very well. This has several implications, stemming from the shared heat between all the printhead components:

- The extruder stepper motor heats up more
- The printhead expands, causing changes in dimensions and alignment
- The hot end heatbreak does not cool as efficiently
- Printed parts and joints to them may warp

Elaborating on the specific components that are most affected by heat in a usual VzBot build, we can see several of the benefits of watercooling the core parts of our printer:

1. Goliath hotend  
    Watercooling your [Goliath] keeps the heatbreak cooler than air cooling. This can prevent clogging and filament jamming, especially when printing in a hot enclosure or printing PLA. Clogging happens when the filament expands inside the heatbreak and jams itself in to the cavity of the heatbreak.

2. Vz-HextrudORT  
    The [Vz-HextrudORT] stepper motor may overheat when the current limit setting is set very high, the enclosure is very hot, or when the printhead or hot end does not cool externally or efficiently with a heatsink fan. This can cause skipped steps, worsening tolerances in the alignment of extruder parts, or even defirmed filament if the extruder gets hot enough.

3. Stepper motors
4. Stepper motor drivers

[Goliath]: /vz-other/goliath
[Vz-HextrudORT]: /vz-other/vz-hextrudort
[Vz-Printhead]: /vz-other/vz-printhead
