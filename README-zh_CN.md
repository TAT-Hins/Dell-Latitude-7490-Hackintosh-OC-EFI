# Dell-Latitude-7490-Hackintosh-OpenCore-EFI

# 中文文档

## 已测试版本

- macOS Ventura 13.6.6

## System Configuration

| 型号     | 戴尔 Latitude 7490                                           |
| -------- | ------------------------------------------------------------ |
| CPU      | Intel® Core™ i7-8650U vPro                                   |
| 显卡     | Intel Corporation UHD Graphics 620                           |
| 硬盘     | KIOXIA (铠侠) RC10 M.2 Nvme PCIE3.0x4 512GB                  |
| 内存     | Samsung (三星) DDR4 2400Hz SO-DIMM 8GB * 2                   |
| 有线网卡 | Intel® i219LM Gigabit Ethernet Controller,10/100/1000 Mb/s Ethernet (RJ-45) |
| 无线网卡 | Intel® Dual-Band Wireless-AC 8265 Wi-Fi + BT4.2 Wireless Card (2x2) (rev 78) |
| 声卡     | Realtek ALC3246                                              |
| USB驱动  | Intel Corporation JHL6340 Thunderbolt 3 USB 3.1 Controller (C step) |
| 触控板   | Dell 081C:00 044E:121F Mouse+Touchpad+圆点                   |
| 键盘     | AT Translated Set 2 Keyboard (0xab41), 14.1 inches Dual Pointing, backlit |
| 屏幕     | Video Bus (Bus:0x19, LNXVIDEO/video/input0)                  |
| 摄像头   | Microdia HD 720p WebCam                                      |
| 扬声器   |                                                              |
| 电池     | Dell KG7VF92                                                 |
| 耳机     | Intel PCH Headphone Mic (ALSA)                               |
| 雷电接口 | Intel Corporation JHL6340 Thunderbolt 3 Bridge (C step)      |
| 雷电接口 | DisplayPort over USB Type-C(optional Thunderbolt 3           |
| 读卡器   | Realtek RTS525A PCI Express Card Reader                      |
| 键盘热键 | Dell WMI Hotkeys (Bus: 0x19)                                 |

### BIOS版本

- **[1.36.0](https://www.dell.com/support/home/en-us/drivers/driversdetails?driverid=rv03k&oscode=biosa&productcode=latitude-14-7490-laptop)**

### Bootloader / OC EFI版本

- **[OpenCore 0.9.9](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.9)**

### SMBIOS型号

- **MacBookPro15,2**
- 基于[GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)生成的PlatformInfo信息

## BIOS设置

- General
  - Boot mode: **UEFI**
  - CSM (Legacy Option) Mode: **Disabled**
- System Configuration
  - SATA Mode: **AHCI**
  - USB Powershare: **Disabled**
- Security
  - TPM 2.0: **On**
- Secure Boot: **Disabled**
  - Secure Boot Mode: **Deployed Mode**
- Intel Software Guard Extensions
  - Intel SGX: **Software Controlled**
- Performance
  - Intel SpeedStep: **Enabled**
  - C-states control: **Enabled**
  - Intel TurboBoost: **Enabled**
  - HT (HyperThread) control: **Enabled**
- Power Management
  - Intel Speed Shift Technology: **Enabled**
- Post Behavior
  - Fast Boot: **Thorough**
- Virtualization support
  - Virtualization: **Enabled**
  - VT-d (VT for Direct I/O): **Enabled**

## 哪些功能可以正常工作

- [x] 核显显示

- [x] 电源管理

- [x] 系统唤醒 / 睡眠 (电脑盖开合 + 热键Fn+Insert)

- [x] 屏幕背光控制

- [x] WiFi (2.4Ghz + 5Ghz)

- [x] 蓝牙（包括音频，已使用 **`HUAWEI FreeBuds 4`**进行测试)

- [x] 触控板光标移动 + 手势 + 小蓝点光标移动 + 左右按钮

  - 启用触控板的**单指左键，双指右键**:

    > `设置` → `触控板` → `轻点来点按` 

- [x] 热键支持 (Fn+F2/F3调整音量，Fn+F11/F12或Fn+S/B调整屏幕亮度)

- [x] 前置摄像头

- [x] 内置扬声器、麦克风 （已测试，设置**layout-id=`17`**）

- [x] USB-C 充电

- [x] USB-C 数据传输 (已使用**移动硬盘**和**`Android File Transfer`**连接手机测试)

- [x] USB 3.0 (复制1.0GB文件耗时3秒左右, **平均速度超过 300MB/s**)

  - 接入符合条件的设备时，可以在**系统报告**中看到识别出**`USB 3.1 Bus`** 

- [x] USB-C 附件 (已使用 **`HUAWEI USB-C 耳机`**进行测试)

- [x] MicroSD卡读卡器

## 哪些功能无法正常工作

- 有线网卡 
  - 卡死黑屏重启问题已解决, 系统正常识别网卡为 **`Intel I219LM4 PCI Express Gigabit Ethernet`**
  - 网口指示灯在网线连接之后点亮几秒钟然后灭掉了
  - 系统中显示有线网络“未连接”
- 二合一3.5mm耳机孔
- 雷电接口
  - 已知bug，暂无修复计划
- Handoff（接力）, Airdrop（隔空投送） & Sidecar（随航）
  - 需要替换成博通的无线网卡

## 哪些功能未经测试

- [ ] CPU Speedstep技术
- [ ] 核显加速
- [ ] HDMI输出 + HDMI音频输出
- [ ] USB-C DP视频输出
- [ ] FileVault 2
- [ ] 指纹传感器 (无硬件，未标配)
- [ ] WWAN 4G卡 (无硬件，未标配)

## 特别感谢

- [CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh](https://github.com/CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh) **(主要参考)**

## Enjoy!

- 如何有任何bug（**最好是已知的修复手段**），欢迎**随时（尽快）联系我**，感激不尽
