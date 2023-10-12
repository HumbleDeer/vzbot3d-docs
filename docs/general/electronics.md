---
layout: default
title: Electronics
description: # This shows up on rich mbeds in e.g. Discord
parent: General info
# slug: # Whatever you'd like the page address to be below general, i.e. docs.vzbot.org/general/<page>/
---

# Electronics

By far the most daunting part of the printer build for many is wiring up the electronics bay of the printer. But fear not, many have preceeded you on this quest!

## A word on safety

{: .danger }
> You will be working with mains voltages (120 VAC / 240 VAC). Always double check to make sure your printer is unplugged and that the capacitors in the power supplies are depleted (check the status LED) before touching any of the electronics.

## Glossary

Working with electrical wiring and electronics can be confusing due to the plethora of acronyms and shorthands used. Here, we go over the most commonly used acronyms and shorthands within the 3D-printing community.

### Wiring glossary

| Term | Description       | Category     | Note                               |
| ---- | ----------------- | ------------ | ---------------------------------- |
| L    | Live              | mains wiring | *no touchy*                        |
| N    | Neutral           | mains wiring |                                    |
| PE   | Protective earth  | mains wiring | Not the same as ground             |
| VCC  | Voltage Collector | DC voltages  | Derived from BJT Collector voltage |
| GND  | Ground            | DC voltages  | a.k.a. Circuit ground              |
| AGND | Analog Ground     | DC voltages  | Used for analog circuitry          |
| VMOT | Motor voltage     | DC voltages  | Voltage for stepper drivers        |

### Electronics glossary

| Term | Description              | Category    | Note                            |
| ---- | ------------------------ | ----------- | ------------------------------- |
| Cap  | Capacitor                | Components  | Stores and releases energy      |
| JST  | Wire terminal            | Terminals   | Japan Solderless Terminal       |
| CSI  | Camera Serial Interface  | Connections | RPi-exclusive camera connector  |
| DSI  | Display Serial Interface | Connections | RPi-exclusive display connector |

## Useful tools

| Tool            | Purpose                       | Importance | Note                            |
| --------------- | ----------------------------- | ---------- | ------------------------------- |
| Ferrules        | Terminating stranded wire     | Medium     |                                 |
| Crimping pliers | Crimping various terminals    | Medium     | Required for JST, Ferrules, etc |
| Soldering iron  | Soldering wire extensions etc | High       | Better than twisting            |

## Wiring

To start you off, here are some miscellaneous tips you might need on your journey:

- You don't need fancy tools to do electronics wiring, but it does make life more easy.
- Practice crimping (JST) connectors and ferrules and make them pass the "tug test"; this will save you a lot of headaches later!
- It is good practice to stick to the wire color conventions specific to your region.  
    You can of course use any wire color you want, but this may make it harder to troubleshoot later.
- Avoid twisting wires together if soldering is an option  
    Twisted wire connections just aren't very durable or safe for high intensity applications.
- Don't use silicone insulated wire in drag chains  
    The excess friction causes the drag chain to not work properly and wear your wires prematurely.

### AC wire color conventions

Different countries have different standards for mains wiring and the used colours, but these are the most prevalent ones you may want to know of:

| Region                   | Live (L)      | Neutral (N)                   | Protective earth (PE)                 |
| ------------------------ | ------------- | ----------------------------- | ------------------------------------- |
| EU, Argentina, Australia | ![brown wire] | ![blue wire]                  | ![green-yellow wire]                  |
| United States            | ![black wire] | ![white wire] or ![grey wire] | ![green wire] or ![green-yellow wire] |
| Canada                   | ![red wire]   | ![white wire] or ![grey wire] | ![green-yellow wire]                  |

### DC wire color conventions

There is no general standard for what colours are used for what voltage node, but there are some key standard colours we like to abide by in the 3D-printing community

| Potential | Symbol | Colour | Note |
| --------- | ------ | ------ | ---- |
| Ground    | GND    | Black  |      |

[brown wire]: /assets/images/general/electronics/wire-brown.png
[blue wire]: /assets/images/general/electronics/wire-blue.png
[green-yellow wire]: /assets/images/general/electronics/wire-green-yellow.png
[black wire]: /assets/images/general/electronics/wire-black.png
[white wire]: /assets/images/general/electronics/wire-white.png
[grey wire]: /assets/images/general/electronics/wire-grey.png
[green wire]: /assets/images/general/electronics/wire-green.png
[red wire]: /assets/images/general/electronics/wire-red.png
