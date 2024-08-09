---
sidebar_position: 3
---

# OpenWear Core

![image-20240809193748467](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240809193748467.png)

## Overview

The Core is a development board in the OpenWear toolkit, designed to facilitate the rapid prototyping of wearable devices. It follows the paradigm of wearable development boards like Lilypad, but with a completely new approach that includes higher performance, wireless connectivity, and quick attachment, making it an ideal choice for wearable projects.

## Details

The Core is equipped with the ESP32-Pico-D4 chip and also has a variety of sensors onboard that can be used for wearable projects, including:

- Power Management Chip (MCP73831T-2ATI/OT): Suitable for lithium polymer batteries, ensuring a reliable power supply.
- Light Sensor (ALS-PT19-315C/L177/TR8): For ambient light detection.
- Temperature and Pressure Sensor (BMP280): For monitoring environmental conditions.
- Six-Axis Gyroscope (LSM6DS3TR): For precise motion recognition.
- RGB LED (WS@218b): For providing visual feedback.

The integration of these sensors allows users to quickly prototype with minimal connections, simplifying the development process.

## Pinout

The Core features 14 pins and supports a variety of communication protocols, including I2C, SPI, and UART. It also includes battery soldering pads on the bottom of the PCB and a Type-C interface for convenient power and data transfer.

![pinout](https://raw.githubusercontent.com/anxndsgn/PicGo/main/pinout.png)

# Qucik Attachment

One standout feature of the OpenWear Core is its innovative magnetic attachment system. Inspired by the quick-release magnetic buckles commonly used in clothing, the board is embedded with two Neodymium (N52) magnets, allowing for quick and secure attachment to fabric without the need for sewing. The accompanying magnetic pads, made from 3D-printed thermoplastic polyurethane (TPU), have six holes: two for embedding the magnets and the remaining four for sewing, offering flexibility in various attachment methods.

![image-20240809194048868](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240809194048868.png)

![image-20240809194206456](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240809194206456.png)

# Schematic

![](https://raw.githubusercontent.com/openwearxyz/PicGo/main/SCH_Schematic_1-Main_2024-08-09.png)

![](https://raw.githubusercontent.com/openwearxyz/PicGo/main/SCH_Schematic_2-Sensor_2024-08-09.png)

## Download

- [Github](https://github.com/openwearxyz/openwear)
- [Core fixing pad 3D printing file](https://github.com/openwearxyz/openwear/blob/main/core%20fixing%20pad.stl)
