# exert cpu

fgpa

## 开发板

### [Sipeed](https://www.sipeed.com/) 荔枝糖 nano 1k (lichee tang nano 1k)

使用的高云的 GW1NZ， 烧录的时候要选 内嵌 Flash 模式（默认是 SRAM）。

注：烧录前按（Run All）编译下。因为编程器是独立的，不会烧录的时候去编译代码。

注：Run All 的时候不会自动保存，所以要记得保存文件，再 Run All 编译。

### [Sipeed](https://www.sipeed.com/) 荔枝糖 nano 20k (lichee tang nano 20k)

使用高云 GW2A-LV18，

## IDE

### gowin ide

Programmer 用于烧录编程

*.fs 是生成的二进制文件，烧录的时候配置路径选中次文件。

*.v 是 verilog 文件，硬件逻辑
*.cst 是物理常量文件，用来配置引脚输出对应。