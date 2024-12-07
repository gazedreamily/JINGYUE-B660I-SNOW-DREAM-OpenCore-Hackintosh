# JINGYUE-B660I-SNOW-DREAM-OpenCore-Hackintosh

![主板](./imgs/Motherboard.png)

### [Engllish](./README.md)

## OpenCore

### [OpenCore 1.0.2](https://github.com/acidanthera/OpenCorePkg)

## 已尝试的系统版本

+ MacOS Sequoia 15.x

## 硬件参考

+ 主板: 精粤 B660I 雪之梦 D4
+ Bios版本: JYI76008 03/10/2023
+ CPU: 英特尔 12代 I5-12490F
+ 内存: 玖合 16G DDR4 3200Mhz * 2
+ 硬盘: 梵想 S500 Pro 2TB
+ 显卡: 华擎 RX6600 CLD ITX 8G GDDR6
+ 声卡: 瑞昱 ALC897
+ 有线网卡: 瑞昱 RTL8125 Gaming 2.5GbE
+ 有线网卡: 瑞昱 RTL8168H/8111H
+ 无线网卡: 英特尔 AX201

## 注意

+ 请使用[OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools)构建SMBIOS
+ 这个EFI内的英特尔网卡驱动 [itlwm.kext](https://github.com/OpenIntelWireless/itlwm/releases)理论上可以兼容MacOS 12-15。请下载[HeliPort.dmg](https://github.com/OpenIntelWireless/HeliPort/releases/download/v2.0.0-alpha/HeliPort.dmghttps://github.com/OpenIntelWireless/HeliPort/releases/download/v2.0.0-alpha/HeliPort.dmg)作为WIFI客户端，而不是使用系统设置内的WIFI。
+ 英特尔网卡不支持隔空投送。

## BIOS 设置
```
高级
    |-- CPU电源管理控制
        |-- CPU锁配置
	        |-- CFG锁定：关闭
	    |-- PCI总线驱动版本     
	        |-- Re-Size BAR Support：Disabled
    |-- CSM配置
	    |-- CSM支持：关闭
		
启动
  |-- 安全启动
    |-- 安全启动：关闭
```

## 鸣谢

感谢[@WuLongMiTaoLaiYiDa](https://github.com/WuLongMiTaoLaiYiDa)大佬大力帮助，让我得以构建此EFI。

可以关注大佬的B站账号[@乌龙蜜桃来一打](https://space.bilibili.com/244390800)，其中有很多通俗易懂的黑苹果教程。如果你觉得有帮助，别忘了给大佬一键三连！

感谢此Q群的帮助。

![QQGroup](./imgs/QRCode.png)
