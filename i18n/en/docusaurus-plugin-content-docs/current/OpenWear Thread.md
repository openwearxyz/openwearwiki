---
sidebar_position: 5
---

# OpenWear Thread

# OpenWear Thread

![image-20240814182808375](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240814182808375.png)

## Overview

The Thread is a connector used to link the Core and the Module. The Thread uses O-type connectors and bolts for connection. There are the following types of Thread:

- Standard Thread: Both ends have O-type connectors, used to connect the development board and modules in the kit.
- Thread with Built-in Resistor: Both ends have O-type connectors, with an internal resistor. This can be used to connect sensors that require a resistor.
- DuPont Thread: One end has a DuPont connector, and the other end has an O-type connector. It can connect the development board to regular Arduino modules not included in the kit.

![image-20240814183242586](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240814183242586.png)

:::tip

We have found that this type of connection may have stability issues, and we are currently exploring new quick-connect methods.。Stay tuned!

:::

## Making a Thread

In this section, we guide you on how to customize the Thread to your desired length.

1. Prepare Materials: This includes 20AWG wire, O-type connectors (5mm outer diameter, 3mm inner diameter), heat shrink tubing, resistors (optional), and a TPU braided protective sleeve (optional, you can pick your sleeve color).
1. Cut the Protective Sleeve and Wire to the required length, then insert the wire into the protective sleeve. Note that the wire should be slightly longer to leave some internal copper wire for soldering.
1. (Optional): If a resistor is needed, solder the resistor to one end of the wire and insert the resistor into the protective sleeve.
1. Solder both ends to the O-type connectors.
1. Cut the Heat Shrink Tubing to about 5mm in length and slide it onto the wire. Use a heat gun to shrink the tubing. Done!
