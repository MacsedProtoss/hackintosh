# hackintosh

## 系统支持

macOS mojave 10.14Beta - 10.14.5(18F132) ——下载Mojave版本

macOS Catalina 10.15Beta2(19A487m) - 10.15.4(19E266) ——下载Catalina版本 可能需要更新clover版本和kext

macOS Catalina 10.15.4(19E266) ——OpenCore版本

## 安装须知

**All：**

* 所有的SMBIOS相关都是随便初始化的，请自行输入数据，可以使用MacSerial来计算

**OpenCore ：**

* 默认开启了开机Chime（登场音效），但是没有配备音频文件，若有需求可以自行下载然后解压到/Resources里面
* 为了Boot Camp和开机热键体验进行了这些修改，安装初期最好去掉这些
  * 默认关闭了-v，请注意安装初期最好开起来
  * 默认不会ShowPicker，建议安装初期启用ShowPicker（否则不会显示引导选项）
  * 默认关闭了AllowSetDefault（允许设置默认引导项）

## 平台简介

HP ZHAN99 WorkStation G1（国行：惠普战99，外行：HP Zbook 15v G5）

### 主要配置

* Intel Core I7-8750h 6C12T
* Crucial DDR4 2666MHz 8G*2
* UHD630 
* Realtek Alc295
* Broadcom BCM94360CS2 （Mac拆机卡+转接m.2卡，我之前用的dw1560现在价格炒得太高了，我卖了还赚了一笔，而且dw1560在Catalina里面蓝牙有问题，现在建议大家买我用的这个了，不过淘宝已经把它从35炒到了100多，真黑心）
* Samsung pm961

### 完成功能

**All:**

* CPU xcpm原生节能控制
* 内建显示器
* UHD630 2048M
* AppleALC驱动声卡
* Wi-Fi（免驱）&AirDrop&SideCar（Sidecar需要Catalina，~~另外可能需要运行几条zsh指令~~，需要保证所有设备登陆同一个Apple ID，**需要iPadOS13配合**）
* 蓝牙（免驱）&handoff 
* 原生电池控制
* 3xUSB3.1接口
* *雷雳三接口（使用HP thunderbolt3 Dock 测试通过）* **可能未被集成进入EFI，请查看下面的阅读链接来自行启用**
* 有线网卡驱动
* 摄像头驱动
* GPS
* 亮度可调
* 触摸板（但是体验一般般，我是直接配合Magic Trackpad 2）
* 睡眠以及唤醒
* 支持iMessage FaceTime App Store iCloud FindMy等功能（需要自己按照要求完善SMBIOS等内容）

**OpenCore**

* 添加了CPUFriend来达到更好的变频效果
* 增加了Chime支持
* 增加了Boot Camp支持 
* 支持直接Recovery在线恢复
* 支持Time Machine直接恢复

### 未完成：

* 指纹无解
* 读卡器没有驱动


### 总体描述：

**基本完美**

### 备注：

* 如果睡眠有问题，请注意检查是否勾选了唤醒以供网络访问
* 我使用的hibernationMod是3


### 阅读链接

[OpenCore CFGLock和部分常见错误](https://macsed.club/2020/03/28/Switch%20to%20OC%20from%20Clover/)

[OpenCore Boot Camp](https://macsed.club/2020/04/05/Opencore-%E6%97%A0%E7%BC%9DBoot-Camp%E5%88%87%E6%8D%A2/)

[OpenCore Chime](https://macsed.club/2020/04/05/Opencore-Chime-%E7%9B%B8%E5%85%B3%E9%97%AE%E9%A2%98/)

[雷电三](https://zhuanlan.zhihu.com/p/75536927)

[Clover Catalina](https://zhuanlan.zhihu.com/p/68774850)

[CLover Mojave](https://zhuanlan.zhihu.com/p/54927820)
