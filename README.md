# [W601](https://doc.soc.xin/W601)

* [winnermicro](http://www.winnermicro.com/): [Cortex-M3](https://github.com/SoCXin/Cortex)
* [L2R2](https://github.com/SoCXin/Level): 80 MHz , [￥6.56](https://item.szlcsc.com/512153.html)

## [简介](https://github.com/SoCXin/W601/wiki)

[W601](https://www.winnermicro.com/html/1/156/158/531.html) Wi-Fi MCU 是一款支持多功能接口的 SoC 芯片。可作为主控芯片应用于智能家电、智能家居、智能玩具、医疗监护、工业控制等物联网领域 。该SoC 芯片集成 Cortex-M3 内核，内置Flash，支持 SDIO、SPI、UART、GPIO、I²C、PWM、I²S、7816、LCD、ADC 等丰富的接口, 支持多种硬件加解密协议，如PRNG/SHA1/MD5/RC4/DES/3DES/AES/CRC/RSA 等；支持 IEEE802.11b/g/n 国际标准。集成射频收发前端RF Transceiver，PA功率放大器，基带处理器/媒体访问控制。


### 关键参数

* 240 MHz Cortex-M3
* 288KB SRAM + 1MB Flash
* 集成1个 SDIO 控制器；
* 集成高速 UART 接口，波特率范围 1200bps~2Mbps
* 集成高速 SPI 控制器，支持速率 20Mbps
* 集成1个 I2C 控制器支持100/400Kbps 速率
* 集成 GPIO 控制器，支持48位可控制 GPIO
* 集成5路 PWM 接口
* 集成双工 I2S 控制器
* 集成7816接口，支持 EVM2000 规范，并兼容串口功能
* 集成 LCD 控制器，支持 4x20/8x16 接口，支持2.7V~3.6V 电压输出
* Wi-Fi4 特性
    * 支持 GB15629.11-2006， IEEE802.11b/g/n
    * 支持 WAPI2.0
    * 支持 Wi-Fi WMM/WMM-PS/WPA/WPA2/WPS
    * 支持 EDCA 信道方式
    * 支持 20/40M 带宽工作模式
    * 支持 STBC、GreenField、Short-GI、支持反向传输
    * 支持 AMPDU、AMSDU
    * 支持 IEEE802.11n MCS0~7、MCS32 物理层传输速率档位，传输速率最高150Mbps
    * 2/5.5/11Mbps 速率发送时支持 Short Preamble
    * 支持 HT-immediate Compressed Block Ack、Normal Ack、No Ack 应答方式
    * 支持 CTS to self
    * 支持 STA、AP、APSTA 功能


## [资源收录](https://github.com/SoCXin)

* [参考资源](src/)
* [参考文档](docs/)
* [参考工程](project/)

## [选型建议](https://github.com/SoCXin/W601)

[W601](https://github.com/SoCXin/W601)与[W806](https://github.com/SoCXin/W806)相比的主要差异在于内核配置，同时没有配置BT/BLE功能。


## [www.SoC.xin](http://www.SoC.Xin)
