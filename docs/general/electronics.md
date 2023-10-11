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

{: .highlight }
> You will be working with mains voltages (120 VAC / 240 VAC). Always double check to make sure your printer is unplugged and that the capacitors in the power supplies are depleted (check the status LED) before touching any of the electronics.

## Wiring

* You don't need fancy tools to do electronics wiring, but it does make life more easy. Practice crimping (JST) connectors and ferrules and make them pass the "tug test"; this will save you a lot of headaches later!
* It is good practice to stick to the wire color conventions specific to your region. You can of course use any wire color you want, but this may make it harder to troubleshoot later.

### AC wire color conventions

| Region | Live | Neutral | Protective earth |
|--------|------|---------|------------------|
| European Union, Argentina, Australia | ![brown wire](/assets/images/general/electronics/wire-brown.png) | ![blue wire](/assets/images/general/electronics/wire-blue.png) | ![green and yellow wire](/assets/images/general/electronics/wire-green-yellow.png) |
| United States | ![black wire](/assets/images/general/electronics/wire-black.png) | ![white wire](/assets/images/general/electronics/wire-white.png) or ![grey wire](/assets/images/general/electronics/wire-grey.png) | ![green](/assets/images/general/electronics/wire-green.png) or ![green and yellow wire](/assets/images/general/electronics/wire-green-yellow.png) |
| Canada | ![red wire](/assets/images/general/electronics/wire-red.png) | ![white wire](/assets/images/general/electronics/wire-white.png) or ![grey wire](/assets/images/general/electronics/wire-grey.png) | ![green and yellow wire](/assets/images/general/electronics/wire-green-yellow.png) |

### DC wire color conventions
