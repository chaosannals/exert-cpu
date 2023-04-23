# exert cpu

fgpa

## 开发板

### [Sipeed](https://www.sipeed.com/) 荔枝糖 nano 1k (lichee tang nano 1k)

使用的高云的 GW1NZ， 烧录的时候要选 内嵌 Flash 模式（默认是 SRAM）。

- Access Mode: Embedded Flash Mode
- Operation: embFlash Erase, Program

### [Sipeed](https://www.sipeed.com/) 荔枝糖 nano 20k (lichee tang nano 20k)

使用高云 GW2A-LV18。

Dock 底板工作 拨下 1 号拨码开关，LED0 LED1 常亮。

烧录选 外置通用 Flash 模式。

- Access Mode: External Flash Mode
- Operation: exFlash Erase, Program thru GAO-Bridge
- Device: Generic Flash
- Start Address: 0x000000

## IDE

### gowin ide

Programmer 用于烧录编程，配置好烧录的方式。

注：烧录前按（Run All）编译下。因为编程器是独立的，不会烧录的时候去编译代码。
注：Run All 的时候不会自动保存，所以要记得保存文件，再 Run All 编译。

*.fs 是生成的二进制文件，烧录的时候配置路径选中次文件。

*.v 是 verilog 文件，硬件逻辑。
*.cst 是物理常量文件，用来配置引脚输出对应。

## 文档与资料

- [Sipeed Wiki](https://wiki.sipeed.com/) Sipeed 板子资料。