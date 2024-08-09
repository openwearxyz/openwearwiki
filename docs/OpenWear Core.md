---
sidebar_position: 3
---

# OpenWear Core

![image-20240809193748467](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240809193748467.png)

## 概览

The Core 是 OpenWear 工具包中的开发板，旨在实现快速的可穿戴原型搭建。它基于像 Lilypad 这样的可穿戴开发板范例，但采用了全新的设计方法，包括更高的性能、无线连接与快速固定，使其成为可穿戴项目的理想选择。

## 技术细节

Core 搭载了 ESP32-Pico-D4 芯片，同时还板载了许多可用于可穿戴项目的传感器，其中包括：

- 电源管理芯片（MCP73831T-2ATI/OT）：适用于锂聚合物电池，确保可靠的电源供应。
- 光敏传感器（ALS-PT19-315C/L177/TR8）：用于环境光检测。
- 温压传感器（BMP280）：用于监测环境条件。
- 六轴陀螺仪（LSM6DS3TR）：用于精确的运动识别。
- RGB LED（WS218b）：用于提供视觉反馈。

这些传感器的集成允许用户以最少的连接进行快速原型制作，简化了开发过程。

## 引脚分布

Core 具有 14 个引脚，支持多种通信协议，包括 I2C、SPI 和 UART。它还包括 PCB 底部的电池焊接引脚和 Type-C 接口，方便进行电源和数据传输。

![pinout](https://raw.githubusercontent.com/anxndsgn/PicGo/main/pinout.png)

# 快速固定

OpenWear Core 的一个突出特点是其创新的磁力附着系统。受服装中常用的快速磁扣的启发，该板嵌入了两个钕铁硼 N52 磁铁，允许快速且安全地附着在织物上，无需缝纫。配套的磁力垫，由 3D 打印的 TPU 制成，有六个孔，其中两个用于嵌入磁铁，其余四个可用于缝纫，提供了多种附着方法的灵活性。

![image-20240809194048868](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240809194048868.png)

![image-20240809194206456](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240809194206456.png)

# 原理图

![](https://raw.githubusercontent.com/openwearxyz/PicGo/main/SCH_Schematic_1-Main_2024-08-09.png)

![](https://raw.githubusercontent.com/openwearxyz/PicGo/main/SCH_Schematic_2-Sensor_2024-08-09.png)

## 下载

- [Github](https://github.com/openwearxyz/openwear)
- [固定片 3D 打印文件](https://github.com/openwearxyz/openwear/blob/main/core%20fixing%20pad.stl)
