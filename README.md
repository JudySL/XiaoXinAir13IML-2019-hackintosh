# XiaoXinAir13IML-2019-hackintosh
# 联想小新 Air 13IML-2019

## 电脑配置

| 规格     | 配置                             | 备注                                    |
| -------- | -------------------------------- | --------------------------------------- |
| 电脑型号 | Lenovo XiaoXin Air 13 IML 集显版 | 2019，可对应S530-13IML                  |
| 操作系统 | macOS Catalina 10.15             | 自用10.15.7，其他未测试                 |
| 处理器   | Intel Core i5-10210U             |                                         |
| 显卡     | Intel UHD Graphics               | UHD 620 (0x9B41)                        |
| 内存     | 16GB LPDDR3                      |                                         |
| 硬盘     | Nvme SSD 512GB                   | 原装Samsung PM981A，已替换TOSHIBA-RC500 |
| 显示器   | 友达AUO5A2D 13.3" FHD 1920×1080  |                                         |
| 声卡     | Realtek ALC 236                  |                                         |
| WI-FI    | Intel Wireless-AC 9560           | 已替换Dell Wireless 1820A               |
| 摄像头   | Integrated Camera                | USB驱动                                 |
| 指纹     | Goodix fingerpeint SGX           | 无法工作                                |

## 使用说明

* 使用前请务必按照黑果小兵关于[Air13IWL中隐藏BIOS推荐设置](https://github.com/daliansky/Lenovo-Air13-IWL-Hackintosh/blob/master/Advanced/ReadMe.md)操作。
* 系统：自用macOS Catalina 10.15.7，稳定性较好，暂不打算升级至Big Sur或Monterey。
* 处理器：自用i5-10210U (CPUID=0x806EC)，无需处理。其他请参考黑果小兵关于

小新Pro13 Wiki中[<b>查看本机CPUID</b>](https://github.com/daliansky/XiaoXinPro-13-hackintosh/wiki/查看本机CPUID)的相关说明

* 显卡：自用为Intel集显 (0x9B41)，config.plist仿冒<kbd>device-id</kbd>:<kbd>3E9B</kbd>，注入<kbd>ig-platform-id</kbd>:<kbd>3E9B0000</kbd>。可修改为其他，具体参考驱动WhateverGreen.kext[英文说明](https://github.com/acidanthera/WhateverGreen/blob/master/Manual/FAQ.GeForce.en.md)或[中文说明](https://github.com/acidanthera/WhateverGreen/blob/master/Manual/FAQ.IntelHD.cn.md)。手边没有2K以上显示器，无法测试外接是否正常。独显版可借鉴这里[<b>显卡</b>](https://github.com/daliansky/Lenovo-Air13-IWL-Hackintosh/blob/master/Advanced/ReadMe.md)中的参数。
* 硬盘：建议更换原装硬盘，仍希望使用PM981A安装可参考[该方法](https://bbs.pcbeta.com/forum.php?mod=viewthread&tid=1867021)。硬盘需注意的问题可查看[这里的<b>安装部分</b>—<b>混搭硬盘</b>](https://github.com/daliansky/XiaoXinPro-13-hackintosh)内容。
* 声卡：现阶段使用的是自编译AppleALC，注入ID为<kbd>Number</kbd>:<kbd>23</kbd>（<kbd>Data</kbd>:<kbd>17000000</kbd>）。如果存在3.5mm耳麦切换异常问题可安装[<b>ALCPlugFix</b>](https://github.com/daliansky/ALCPlugFix)声卡守护进程处理。
* Wi-Fi：已更换DW1820A。使用Intel无线网卡参考[<b>下面</b>](https://github.com/daliansky/XiaoXinPro-13-hackintosh/wiki/Intel网卡)的说明。
* 该EFI大部分借鉴于黑果小兵的Air13IWL的EFI，仅供参考，相同机型可使用调试，不保证完美，具体请自行测试，之后主要以更新kext为主。

## 鸣谢

* **Acidanthera** 提供 [OpenCore](https://github.com/acidanthera/OpenCorePkg) 和 [相关驱动](https://github.com/acidanthera)
* [Apple](https://www.apple.com/) 开发的 [macOS](https://www.apple.com/macos)
* [<b>黑果小兵</b>](https://github.com/daliansky)维护的[小新Air13IWL](https://github.com/daliansky/Lenovo-Air13-IWL-Hackintosh)和[小新Pro13](https://github.com/daliansky/XiaoXinPro-13-hackintosh)
* **宪武** 提供 [OC-little](https://github.com/daliansky/OC-little)
* [<b>stevezhengshiqi</b>](https://github.com/stevezhengshiqi) 开发的 [one-key-cpufriend](https://github.com/stevezhengshiqi/one-key-cpufriend)
* [<b>litxia</b>](https://github.com/lietxia)维护的[小新Air-14 2019IML](https://github.com/lietxia/XiaoXinAir14IML_2019_hackintosh)
