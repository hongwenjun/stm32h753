## STM32 Nucleo-144开发板 MCU的文档 [STM32H743ZI](https://www.st.com/zh/microcontrollers-microprocessors/stm32h743zi.html#resource) [STM32H753ZI](https://www.st.com/en/evaluation-tools/nucleo-h753zi.html)
- 短域名: https://git.io/stm32
- 采用STM32H743ZI/STM32H753ZI MCU的STM32 Nucleo-144开发板，支持Arduino，ST Zio和morpho连接

![](https://github.com/hongwenjun/stm32h753/raw/master/img/stm32_nucleo.jpg)

## C51单片机  STM32单片机  HC6800-ES V2.0光盘资料 [阿里云盘分享](https://www.aliyundrive.com/s/rn4f6h4cpSr)

### 技术文档手册 资源  [百度网盘链接:](https://pan.baidu.com/s/1MZqNVB_GOtdjwHJQhqx_3Q)   提取码: x1sc

- 产品规格 技术文档 手册 [官方下载](https://www.st.com/zh/microcontrollers-microprocessors/stm32h743zi.html#resource)
- https://www.st.com/zh/microcontrollers-microprocessors/stm32h743zi.html#resource
- https://www.st.com/zh/evaluation-tools/nucleo-h753zi.html

### 概述

- STM32 Nucleo-144板为用户提供了一种经济实惠且灵活的方式，可以通过选择STM32微控制器提供的各种性能和功耗特性组合来尝试新概念和构建原型。对于兼容板，内部或外部SMPS可显着降低运行模式下的功耗。

- 扩展Arduino™Uno V3连接的ST Zio连接器和ST morpho接头提供了一种扩展Nucleo开放式开发平台功能的简便方法，具有多种专用屏蔽选择。
STM32 Nucleo-144板不需要任何单独的探头，因为它集成了ST-LINK调试器/编程器。
STM32 Nucleo-144板带有STM32综合免费软件库和STM32Cube MCU封装的示例。

### 主要特性

- 共同特征

	采用LQFP144封装的STM32微控制器
	
	3个用户LED
	
	2个用户和重置按钮
	
	32.768 kHz晶体振荡器
	
	板连接器：社署ST Zio扩展连接器，包括Arduino™ Uno V3ST morpho扩展连接器
	
	灵活的电源选项：ST-LINK，USB Vbus或外部源
	
	具有USB重新枚举功能的板载ST-LINK调试器/编程器：大容量存储器，虚拟COM端口和调试端口
	
	STM32Cube MCU封装提供全面的免费软件库和示例
	
	多种可供选择的集成开发环境（IDE），包括IAR™，Keil公司的支持?基于GCC和IDE

- 特定于电路板的功能

	外部或内部SMPS生成V 核逻辑电源
	
	以太网符合IEEE-802.3-2002标准
	
	USB OTG全速或仅限设备
	
	板连接器：带Micro-AB或USB Type-C™的USB以太网RJ45
	
	手臂® Mbed启用™兼容
	
### STM32_Nucleo-144开发板 接口图

![](https://github.com/hongwenjun/stm32h753/raw/master/img/nucleo144.jpg)

--- 
## 开发工具和编译环境搭建  [百度网盘链接:](https://pan.baidu.com/s/1nF86J4iN1ICV01TrQHr0DA)   提取码: gw2z 

### 编译环境安装程序 mdk528a.exe 
```
安装 Keil uVision5 和 ARM 编译器后
.\Arm\Packs\.Download\ 会自动安装 UNPACK
ARM.CMSIS.5.5.1.pack 
ARM.CMSIS-Driver.2.4.0.pack 
Keil.ARM_Compiler.1.6.1.pack
Keil.MDK-Middleware.7.8.0.pack
```

### 开发库程序和文档 STM32H7xx_DFP
```
Keil.STM32H7xx_DFP.2.3.0.pack
可以在线安装，如果速度慢，使用这个离线包
放到 .\Arm\Packs\.Download\ 目录下 UNPACK 安装
```

![](https://raw.githubusercontent.com/hongwenjun/stm32h753/master/img/Keil_STM32H7xx_DFP.png)

### 固件下载程序和ST LINK V3驱动
en.stm32cubeprog.zip  释放安装后找到，找到程序目录下的驱动目录安装ST LINK V3驱动

![](https://raw.githubusercontent.com/hongwenjun/stm32h753/master/img/st_link_v3.png)

### 编译库文档示例程序大集成包，不是必须
en.stm32cubeh7.zip 和上面安装的大多数重复

![](https://raw.githubusercontent.com/hongwenjun/stm32h753/master/img/stm32cubeh7.png)
---

## STM32 Nucleo-144 开发板 STM32H743ZI2 示例程序  项目建立和编译编辑 [图文链接](https://github.com/hongwenjun/stm32h753/tree/master/Examples)

### 精选视频

- [用于STM32的Nucleo-32板的产品概述](https://www.st.com/zh/evaluation-tools/nucleo-h743zi.html)

	本视频将展示Nucleo，Nucleo-32并提供有关Nucleo-32的详细信息。Nucleo 32针结构紧凑，但屏蔽板较少。

- [使用STM32 ODE可以更快地进行原型设计和开发](https://www.st.com/zh/evaluation-tools/nucleo-h753zi.html)

	STM32开放式开发环境是开发创新设备和应用程序的灵活，简单且经济实惠的方式。它基于STM32 Nucleo板和STM32Cube软件。

### 以太网物理接口和RJ45连接器

![](https://github.com/hongwenjun/stm32h753/raw/master/Ethernet_PHY/Ethernet_PHY.webp)

- 采用HP Auto-MDIX和flexPWR®技术的小尺寸RMII 10/100以太网收发器  文档: [DS_LAN8742A.pdf](https://github.com/hongwenjun/stm32h753/raw/master/Ethernet_PHY/DS_LAN8742A.pdf)

- Small Footprint RMII 10/100 Ethernet Transceiver with HP Auto-MDIX and flexPWR® Technology

- KMS-1102NL 网络变压器   文档: [H1102NL-rev.A_Model.pdf](https://github.com/hongwenjun/stm32h753/raw/master/Ethernet_PHY/H1102NL-rev.A_Model.pdf)

- TVS瞬态电压抑制二极管 / 极低电容ESD保护  USBLC6-4SC6  文档: [USBLC6-4SC6_datasheet.pdf](https://github.com/hongwenjun/stm32h753/raw/master/Ethernet_PHY/USBLC6-4SC6_datasheet.pdf)

USBLC6-4SC6是一种专用于高速静电放电保护的单片应用离散型接口，如USB2.0、以太网和视频线，
极低的线电容确保了高水平的信号完整性，同时不影响保护敏感芯片免受最强烈的静电放电冲击。
