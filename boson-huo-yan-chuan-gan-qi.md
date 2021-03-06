# 火焰传感器

## 实物图片

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-shi-wu-tu-pian.jpg)

## 基本信息

中文名称：火焰传感器

英文名称：Flame Sensor

序号：i7

SKU：BOS0007

## 功能简介

火焰传感器是机器人专门用来搜寻火源的传感器，也可以用来检测光线的亮度，但本传感器对火焰特别灵敏。火焰传感器主要应用于火灾消防系统，尤其是一些易燃易爆场所，用来检测火焰的产生；此外，该传感器也可以用于发动机、锅炉、窑炉等的火焰报警系统。

## 使用说明

这款火焰传感器可以用来探测火源或其它波长在760纳米～1100纳米范围内的光源，探测角度可达60度，能在-25到85摄氏度下工作，性能稳定可靠。

> * 当火焰增强时，输出信号随之增强；当火焰减弱时，输出信号随之减弱。

按照下图所示连接电路，通电后即可通过火焰传感器控制蜂鸣器模块：当检测到火焰时，蜂鸣器开始鸣叫；否则蜂鸣器停止鸣叫。

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-shi-yong-shuo-ming.png)

**\*注意：**尽管这款传感器用于感知火焰的，但它并不防火。因此使用时请与火焰保持距离，以免烧坏传感器。\*

## 原理介绍

火焰的热辐射具有离散光谱的气体辐射和连续光谱的固体辐射。不同燃烧物的火焰辐射强度、波长分布有所差异，但总体来说，其对应火焰温度的近红外波长域及紫外光域有很大的辐射强度，火焰传感器就是根据这种特性制作而成。 火焰传感器利用红外线对对火焰非常敏感的特点，使用特制的红外线接收管检测火焰，然后把火焰的亮度转化为高低变化的电平信号，输入到中央处理器中，中央处理器根据信号的变化做出相应的程序处理。 来源：[https://baike.baidu.com/item/火焰传感器/8405773?fr=aladdin](https://baike.baidu.com/item/火焰传感器/8405773?fr=aladdin)

## 应用样例

### \(1\) 火灾报警器

**样例说明：**当发生火灾的时候，火焰传感器感知到火焰，蜂鸣器模块发出警报。

**元件清单：**火焰传感器；电源主板-三路；蜂鸣器模块。

**连线图：**

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-ying-yong-yang-li-1-lian-xian-tu.png)

### \(2\) 火炉自动报警器

**样例说明：**火炉点火后，火焰传感器开始检测，若燃气灶火焰熄灭，火焰传感器传回信号，蜂鸣器报警。

**元件清单：**火焰传感器；逻辑“非”模块；电源主板-单路；蜂鸣器模块。

**连线图：**

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-ying-yong-yang-li-2-lian-xian-tu.png)

### \(3\) 灭火机器人

**样例说明：**当发生火灾的时候，火焰传感器检测到火焰后迅速使用风扇扑灭火焰。

**元件清单：**火焰传感器；风扇模块；蜂鸣器模块；Micro:bit；Micro:bit BOSON扩展板。

**连线图：**

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-ying-yong-yang-li-3-lian-xian-tu.png)

**设计意图：**由于火焰传感器的输出信号是模拟值，这里设置一个临界值“30”（临界值需要根据环境等因素经过多次测试后确定），当火焰传感器输出模拟值大于30时表示发生火情，蜂鸣器和风扇开始工作，否则关闭蜂鸣器和风扇。

**执行流程：**

① 已发生火情：若火焰传感器检测到火焰，蜂鸣器发出警报声，打开风扇开始灭火并持续5秒；

② 未发生火情：若火焰传感器没有检测到火焰，关闭蜂鸣器和风扇。

**程序示意图（中文版）：**

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-ying-yong-yang-li-3-cheng-xu-shi-yi-tu-zhong-wen-ban.png)

**程序示意图（英文版）：**

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-ying-yong-yang-li-3-cheng-xu-shi-yi-tu-ying-wen-ban.png)

## 参数规格

引脚说明：

![](.gitbook/assets/boson-huo-yan-chuan-gan-qi-yin-jiao-shuo-ming.png)

重量： （g）

尺寸：26mm\*22mm

工作电压：3.0-5.0V

