# hackintosh

## 系统支持

macOS mojave 10.14Beta - 10.14.5(18F132) ——下载Mojave版本

macOS Catalina 10.15Beta2(19A487m) - 10.15.4(19E266) ——下载Catalina版本 可能需要更新clover版本和kext

macOS Catalina 10.15.4(19E266) ——OpenCore版本

## 安装须知

请输入MLB ROM自己的等数据可以使用MacSerial来计算

OpenCore 默认开启了开机Chime（登场音效），但是没有配备音频文件，若有需求可以自行下载然后解压到/Resources里面。

## 平台简介

HP ZHAN99 WorkStation G1（国行：惠普战99，外行：HP Zbook 15v G5）

### 主要配置

* Intel Core I7-8750h 6C12T
* Crucial DDR4 2666MHz 8G*2
* UHD630 
* Realtek Alc295
* Broadcom BCM94360CS2 （Mac拆机卡+转接m.2卡，我之前用的dw1560现在价格炒得太高了，我卖了还赚了一笔，而且dw1560在Catalina里面蓝牙有问题，现在建议大家买我用的这个了，不过淘宝已经把它从35炒到了100多，真黑心）
* Samsung pm961

### 拓展坞

* HP thunderbolt3 Dock


### 完成功能

**Mojave&Catalina:**

* CPU xcpm原生节能控制
* 内建视网膜显示器（内建OK，视网膜要自己运行脚本）
* UHD630 2048M
* AppleALC驱动声卡
* Wi-Fi（免驱）&AirDrop&SideCar（Sidecar需要Catalina，另外可能需要运行几条zsh指令，需要保证所有设备登陆同一个Apple ID，**需要iPadOS13配合**）
* 蓝牙（免驱）&handoff 
* 原生电池控制
* 3xUSB3.1接口
* 雷雳三接口（使用HP thunderbolt3 Dock 测试通过）
* 有线网卡驱动
* 摄像头驱动
* GPS
* 开机不会无背光
* 亮度可调
* 触摸板
* 睡眠以及唤醒


### 未完成：


* 指纹无解
* 读卡器没有驱动


### 总体描述：

**基本完美**

### 安装须知：

* SMBIOS部分上传之前已经随机生成 大家请记得去参照启用iMessage和FaceTime的方法去配置自己的smbios、rt variable 之类的地方，实测是可以完美的（需要BCM94360CS2支持）

* 如果睡眠有问题，请注意检查是否勾选了唤醒以供网络访问


### 阅读链接

[OpenCore](https://macsed.club/2020/03/28/Switch%20to%20OC%20from%20Clover/)

[雷电三](https://zhuanlan.zhihu.com/p/75536927)

[Catalina](https://zhuanlan.zhihu.com/p/68774850)

[Mojave](https://zhuanlan.zhihu.com/p/54927820)
