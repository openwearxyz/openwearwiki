---
sidebar_position: 5
---

# OpenWear Thread

![image-20240814182808375](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240814182808375.png)

## 概览

Thread是用来连接Core与Module的连接线。Thread采用了O型连接器与螺栓来进行连接。Thread主要有以下一种型号：

* 普通Thread。两头均为O型连接器，用于连接套件中的开发板与模块。
* 内部带有电阻的Thread。两头均为O型连接器，内部有电阻，可用于连接某些要求使用电阻的传感器。
* 杜邦线Thread。一端是杜邦线连接器，另一端是O型连接器。可以连接开发板与不包含在套件中的普通Arduino模块。

![image-20240814183242586](https://raw.githubusercontent.com/openwearxyz/PicGo/main/image-20240814183242586.png)

:::tip

我们发现此种连接方式可能会存在连接不稳定的问题，我们正在寻找新的快速连接方法。Stay tuned!

:::

## 制作Thread

在此节中，我们指导你如何定制所需长度的Thread。

1. 准备材料。包括 20AWG规格的电线、O型连接器（外径5mm，内径3mm）、热缩管、电阻（可选），TPU针织保护套（可选）。
1. 将保护套与电线裁剪到需要的长度，之后将电线伸入套护套中。注意电线应该稍长，预留出用于焊接的内部铜线。
1. （可选）如果需要电阻，则将电阻焊接到电线一端，将电阻伸入保护套。
1. 将两端焊接到O型连接器上。
1. 将热缩管裁剪到大约5mm长，套入热缩管。使用热风枪将热缩管加热。完成！
