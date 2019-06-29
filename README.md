# hackintosh

## 系统支持

macOS mojave 10.14Beta - 10.14.5(18F132) ——下载Mojave版本
macOS Catalina 10.15Beta(19A487m) ——下载Catalina版本

## 平台简介

HP ZHAN99 WorkStation G1（惠普战99）

### 主要配置

* Intel Core I7-8750h 6C12T
* Crucial DDR4 2666MHz 8G*2
* UHD630 （N卡已凉）
* Realtek Alc295
* Broadcom BCM94360CS2 （Mac拆机卡+转接m.2卡，我之前用的dw1560现在价格炒得太高了，我卖了还赚了一笔，而且dw1560在Catalina里面蓝牙有问题，现在建议大家买我用的这个了，不过淘宝已经把它从35炒到了100多，真黑心）
* Samsung pm961

### 完成功能

**Mojave&Catalina:**

* CPU12阶睿频
* 内建视网膜显示器（内建OK，视网膜要自己运行脚本）
* UHD630 2048M
* AppleALC驱动声卡
* Wi-Fi（免驱）&AirDrop&SideCar（Sidecar需要Catalina，另外可能需要运行几条zsh指令，需要保证所有设备登陆同一个Apple ID，**需要iPadOS13配合**，**有线模式必须使用C To L的线**）
* 蓝牙（免驱）&handoff 
* 原生电池控制
* USB3.1&typeC （雷雳可驱动但是效果不好我删掉了 要驱动的话只要根据IOElectricity来做就行了）
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
* 暂时不release雷雳的驱动


### 总体描述：

**基本完美**

### 安装须知：

smbios部分上传之前已经随机生成 大家请记得去参照启用iMessage和FaceTime的方法去配置自己的smbios、rt variable 之类的地方，实测是可以完美的（需要BCM94360CS2支持）


