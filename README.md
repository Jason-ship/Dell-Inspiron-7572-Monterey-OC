# 适用于Dell Inspiron 7572笔记本安装与运行macOS Big Sur的OpenCore EFI配置
  * 更新：2021年4月9日
  * 更新内容：
  * OpenCore 0.6.9 =====> OpenCore 0.7.0
# 注意：该EFI文件只适用于Big Sur版本。
# 本EFI配置思路基于[@ic005k](https://github.com/ic005k)的[Dell Inspiron 7472 OC配置文件](https://github.com/ic005k/DELL7472)
* 如需运行Catalina版本，请使用 [@Lyn](https://github.com/lyngogogog)的 [EFI](https://github.com/lyngogogog/Dell-7472-7572-Hackintosh-EFI)配置文件。
* 如若安装更低版本的macOS，可以使用[@黑果小兵](https://github.com/daliansky)的[CLOVER配置文件](https://github.com/daliansky/Dell-Inspiron-7560-Hackintosh)
# >>>[点击此处下载EFI配置文件(Github) 网络问题，暂未上传Release包](https://github.com/iXeor/Dell-Inspiron-7572-BigSur-OC/releases/download/Dell-Ins-7572-BigSur-OC-6.9-RELEASE/EFI.zip)<<<
# >>>[点击此处下载EFI配置文件(Gitee)](https://gitee.com/Shirakage/Dell-Inspiron-7572-BigSur-OC/attach_files/709779/download/EFI.zip)<<<
## 电脑配置

| 规格     | 详细信息                                                     |
| -------- | ------------------------------------------------------------ |
| 电脑型号 | 戴尔 Inspiron 7572 笔记本电脑                                |
| BIOS版本 | Inspiron_7472_7572_1.6.1                               |
| 操作系统 | macOS Big Sur 11.3.1/Windows 10 专业工作站版Dev 21387/Ubuntu 20.10       |
| 处理器   | Intel Core i5-8250U @ 1.80GHz 四核八线程                          |
| 内存     | 16 GB ( 科赋 DDR4 2400MHz )                                |
| 硬盘1     | 三星 970 EVO (250 GB / 固态硬盘 )                          |
| 硬盘2     | HGST HTS541010B7E610 (1 TB / 机械硬盘 )                          |
| 显卡1     | 英特尔 HD Graphics 620 （保留2 GB显存）             |
| 显卡2     | NVIDIA MX 150 4G（未使用）              |
| 显示器   | BOE(京东方) NV156FHM-H61 FHD 1920x1080 (15.6 英寸)                       |
| 声卡     | ALC256 (layout-id:2/56)                                      |
| 网卡     | Intel Wi-Fi 6 AX200 160MHz                      |
| OpenCore版本     | OpenCore-0.7.0-RELEASE                      |

## 特性

* 集成[OpenIntelWireless](https://github.com/OpenIntelWireless)的[itlwm](https://github.com/OpenIntelWireless/itlwm)、[IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)和[AirportItlwm](https://github.com/OpenIntelWireless/itlwm/tree/master/AirportItlwm)，可以使用一部分Intel品牌的无线网卡
* 支持将macOS Big Sur安装到机械硬盘
* 引导界面可以关机或重启

## 目前已知问题与解决方法：

* 耳机插口失效问题：安装[ComboJack](https://github.com/hackintosh-stuff/ComboJack)以解决
* SD卡卡槽暂时不能读取SD卡（待解决）
* 如出现实装EFI后不能正常关机、时间错误的情况，可以通过安装Linux解决
* 在安装第二、三阶段出现偶发性花屏属正常现象，待其自动重启即可
* 使用本EFI配置不能启动低版本的macOS（会出现禁止符号），暂无解决办法
* CPU原生支持，变频正常
* 显示器亮度调节正常；
* 使用博通（Boardcom）品牌的网卡的大佬麻烦禁用'itlwm.kext'和'AirportItlwm.kext',并在'boot-args'中添加'brcmfx-country=#a brcmfx-driver=2'


## 更新 2022 Mac OS Monterey
电脑型号               戴尔 Inspiron 7572 笔记本电脑
  操作系统               Windows 10 专业版 64位（Version 21H2 / DirectX 12）

  处理器                 英特尔 Core i5-8250U @ 1.60GHz 四核
  主板                   戴尔 04JMR2（7th/8th Generation Intel Processor Family I/O - 9D4E 笔记本芯片组）
  显卡                   NVIDIA GeForce MX150 ( 4 GB / 戴尔 )
  内存                   16 GB ( 威刚 DDR4 2400MHz )
  主硬盘                  PC SN520 NVMe WDC 256GB ( 256 GB / 固态硬盘 )
  显示器                 京东方 BOE06B4 ( 15.5 英寸  )
  声卡                   瑞昱  @ 英特尔 High Definition Audio 控制器
  网卡                   瑞昱 RTL8168/8111/8112 Gigabit Ethernet Controller / 戴尔

* 显示器亮度调节不正常
* 博通网卡BCM4360 可正常使用
* 无其他问题
EFI 下载 https://wwn.lanzoul.com/iLHAizijfkh
链接:https://pan.baidu.com/s/1Q53D7lyZVgiJmt4ESDm6cg 提取码:1k7d 复制这段内容后打开百度网盘手机App，操作更方便哦
# 注意：该EFI文件只适用于Monterey版本。
