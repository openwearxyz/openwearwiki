---
sidebar_position: 2
---
在使用OpenWear开始之前，你需要准备编写代码的环境。OpenWear Core支持使用Arduino和MicroPython进行编程，你可以选择你熟悉的语言编写代码。
## 准备编程环境

### 使用 Arduino
要使用 Arduino IDE 编写代码，你首先需要下载并安装 Arduino IDE。如果你尚未安装 Arduino IDE，请访问 [Arduino 官网](https://www.arduino.cc/en/software) 进行下载安装。安装完成后，访问 [OpenWear GitHub 仓库](https://github.com/anxndsgn/OpenWear) 并下载源码（点击 `Code -> Download ZIP`），解压后你将找到名为 `Arduino Board ESP32 Variants` 的文件夹。

![](https://raw.githubusercontent.com/anxndsgn/PicGo/main/20231208023145.png?token=AOQBL6N3VDFEUIHC6G5VPDTFOIH5A)

安装 IDE 后，下一步是安装 ESP32 开发板支持包。

* 对于 Windows 系统，依次点击 `文件 -> 首选项`；
* 对于 macOS 系统，依次点击 `Arduino IDE -> 首选项`。
  

在“其他开发板管理器 URLs”处输入 `https://espressif.github.io/arduino-esp32/package_esp32_index.json`。然后打开开发板管理器，搜索 `esp32` 并安装。具体安装步骤可参考 [Espressif 官方教程](https://espressif-docs.readthedocs-hosted.com/projects/arduino-esp32/en/latest/installing.html)。

![image-20231212235302511](https://raw.githubusercontent.com/anxndsgn/PicGo/main/202312122353567.png)

![image-20231212235406862](https://raw.githubusercontent.com/anxndsgn/PicGo/main/202312122354026.png)

在完成安装后，

* 对于 Windows 系统，打开文件管理器并导航至`C:\Users\你的用户名\AppData\Local\Arduino15\packages\esp32\hardware\esp32\版本号`；
* 对于 macOS，打开 Finder 并导航至 `/Users/你的用户名/Library/Arduino15/packages/esp32/hardware/esp32/版本号`。

将 `Arduino Board ESP32 Variants` 文件夹中的 `openwear_pico` 文件夹复制到 `variants` 文件夹中。接下来，打开 `boards.txt` 文件，将 `openwear_pico.txt` 中的内容复制粘贴到 `boards.txt` 文件的末尾，保存并退出。完成以上步骤后，重新打开 Arduino IDE，你应该能够在开发板列表中找到 OpenWear 开发板。

![](https://raw.githubusercontent.com/anxndsgn/PicGo/main/20231208025000.png)

### 使用MicroPython

对于使用[MicroPython](https://micropython.org/)的用户，请使用[Thonny](https://thonny.org/)编写并烧录代码。OpenWear提供具有MicroPython固件的开发板，如果你的开发板正在使用Arduino IDE，请先烧录固件。你可以使用Thonny烧录固件，烧录固件教程在[这里](https://randomnerdtutorials.com/getting-started-thonny-micropython-python-ide-esp32-esp8266/#:~:text=Flashing%20MicroPython%20Software)。使用Thonny烧录代码可以参考[这里](https://randomnerdtutorials.com/getting-started-thonny-micropython-python-ide-esp32-esp8266/)。

想要使用openwear的引脚定义，请先参考Arduino一节下载Github代码。解压后你会得到`MicroPython Pin Def`文件夹，将`openwearpin.py`文件使用Thonny打开，点击`文件->另存为->MicroPython设备中`，保存为`opnwearpin.py`。

![Snipaste_2023-12-12_23-33-13](https://raw.githubusercontent.com/anxndsgn/PicGo/main/202312122349247.png)

或者也可以新建名为`openwearpin.py`文档，拷贝下列代码，点击保存。

```python
# This file contains the pin mapping for the OpenWear board
# use 'import openwearpin' in your code to access the pins
# e.g. openwearpin.A0

A0 = 4
A1 = 2
A2 = 18
A3 = 23
A4 = 25
A5 = 26
A6 = 27
A7 = 14
A8 = 12
A9 = 13
A10 = 15
SCL1 = 18
SDA1 = 23
```

在编写代码时，在主代码中`import openwearpin`。

示例：

```python
import openwearpin
from machine import Pin

p0 = Pin(openwearpin.A0, Pin.OUT)    # create output pin on A0
p0.on()                 # set pin to "on" (high) level
p0.off()                # set pin to "off" (low) level
p0.value(1)             # set pin to on/high

p2 = Pin(openwearpin.A1, Pin.IN)     # create input pin on A1
print(p2.value())       # get value, 0 or 1
```



## 安装驱动文件

:::tip

如果在完成上述步骤后无法上传代码（特别是macOS），请考虑安装相应驱动。[下载链接](https://www.wch.cn/products/CH343.html#:~:text=%E5%9B%BE%EF%BC%9ASCHPCB.ZIP-,3.%20%E9%A9%B1%E5%8A%A8,-Windows%20%E5%8E%82%E5%95%86VCP)。

:::



