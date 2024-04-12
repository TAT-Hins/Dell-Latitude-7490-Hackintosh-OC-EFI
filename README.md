# Dell-Latitude-7490-Hackintosh-OpenCore-EFI

- Readme translation: **[English]()|[中文文档]()**

------

# English

## Tested macOS Version

- macOS Ventura 13.6.6


## System Configuration

| Model | Dell Latitude 7490 |
| --- | --- |
| CPU | Intel® Core™ i7-8650U vPro |
| Graphic | Intel Corporation UHD Graphics 620 |
| Hard Drive | KIOXIA EXCERIA RC10 M.2 Nvme PCIE3.0x4 500GB |
| RAM | Samsung (三星) DDR4 2400Hz SO-DIMM 8GB * 2 |
| Ethernet | Intel® i219LM Gigabit Ethernet Controller,10/100/1000 Mb/s Ethernet (RJ-45) |
| Wireless | Intel® Dual-Band Wireless-AC 8265 Wi-Fi + BT4.2 Wireless Card (2x2) (rev 78) |
| Sound Card | Realtek ALC3246  |
| USB | Intel Corporation JHL6340 Thunderbolt 3 USB 3.1 Controller (C step) |
| Touchpad | Dell 081C:00 044E:121F Touchpad + Trackpad + Trackpoint |
| Keyboard | AT Translated Set 2 Keyboard (0xab41), 14.1 inches Dual Pointing, backlit |
| Screen | Video Bus (Bus:0x19, LNXVIDEO/video/input0) |
| Camera | Microdia HD 720p WebCam |
| Speaker |  |
| Battery | Dell KG7VF92/F3YGT |
| Thunderbolt | Intel Corporation JHL6340 Thunderbolt 3 Bridge (C step) |
| Thunderbolt | DisplayPort over USB Type-C(optional Thunderbolt 3 |
| Card Reader | Realtek RTS525A PCI Express Card Reader |
| Hotkeys | Dell WMI Hotkeys (Bus: 0x19) |

### BIOS Version

- **[1.36.0](https://www.dell.com/support/home/en-us/drivers/driversdetails?driverid=rv03k&oscode=biosa&productcode=latitude-14-7490-laptop)**

### Bootloader / OC EFI Version

- **[OpenCore 0.9.9](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.9)**

### SMBIOS model

- **MacBookPro15,2**
- Generated PlatformInfo based on [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)


## BIOS Settings

- Boot mode: UEFI
- Fast Boot: Thorough
- SecureBoot: Disable
- SATA Mode: AHCI 
- Intel SGX: Software Controlled


## What's working

- [x] iGPU displaying
- [x] Battery Management
- [x] Wake / Sleep (Lid & Fn + Insert)
- [x] Screen backlight
- [x] WiFi (2.4Ghz + 5Ghz)
- [x] Bluetooth (Including Audio)
- [x] Touchpad with Gestures + Trackpad + Buttons
  - Enable **Touchpad click button (single for left click / double for right click)**:
    `System Settings` → `Trackpad` → `Tap to click`
- [x] Native hotkeys support with Fn keys (Volume Fn+F2/F3 and Screen Brightness Fn + F11/F12)
- [x] USB-C charging

## What's not working

- Audio / Internal Speakers (needs to test **layout-id** for **`AppleALC`**)
- Ethernet (needs to test IntelMausi.kext)
- Thunderbolt (Known issues, not planning to fix currently)
- Handoff, Airdrop & Sidecar (needs to replace a Broadcomm wireless adapter)


## What's not tested yet

- [ ] 2-in-1 3.5mm headphone jack
- [ ] CPU Speedstep
- [ ] iGPU acceleration
- [ ] Internal Microphone
- [ ] HDMI + audio over HDMI
- [ ] Web Camera
- [ ] USB 3.0
- [ ] MicroSD card reader (No SD card here)
- [ ] USB-C DP-alt Mode
- [ ] USB-C Data transfer
- [ ] FileVault 2
- [ ] Fingerprint sensor (No hardware, SKU not included)
- [ ] Smart card reader (No hardware, SKU not included)
- [ ] WWAN card (No hardware, SKU not included)


## Special credits

- [CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh](https://github.com/CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh) **(Mostly as referenced)**


## Enjoy!

- Please **let me know ASAP** if there're any bugs that can be fixed

------

# 中文文档

## 已测试版本

- macOS Ventura 13.6.6

## System Configuration

| 型号 | 戴尔 Latitude 7490 |
| --- | --- |
| CPU | Intel® Core™ i7-8650U vPro |
| 显卡 | Intel Corporation UHD Graphics 620 |
| 硬盘 | KIOXIA (铠侠) RC10 M.2 Nvme PCIE3.0x4 512GB |
| 内存 | Samsung (三星) DDR4 2400Hz SO-DIMM 8GB * 2 |
| 有线网卡 | Intel® i219LM Gigabit Ethernet Controller,10/100/1000 Mb/s Ethernet (RJ-45) |
| 无线网卡 | Intel® Dual-Band Wireless-AC 8265 Wi-Fi + BT4.2 Wireless Card (2x2) (rev 78) |
| 声卡 | Realtek ALC3246  |
| USB驱动 | Intel Corporation JHL6340 Thunderbolt 3 USB 3.1 Controller (C step) |
| 触控板 | Dell 081C:00 044E:121F Mouse+Touchpad+圆点 |
| 键盘 | AT Translated Set 2 Keyboard (0xab41), 14.1 inches Dual Pointing, backlit  |
| 屏幕 | Video Bus (Bus:0x19, LNXVIDEO/video/input0) |
| 摄像头 | Microdia HD 720p WebCam |
| 扬声器 |  |
| 电池 | Dell KG7VF92 |
| 耳机 | Intel PCH Headphone Mic (ALSA) |
| 雷电接口 | Intel Corporation JHL6340 Thunderbolt 3 Bridge (C step) |
| 雷电接口 | DisplayPort over USB Type-C(optional Thunderbolt 3 |
| 读卡器 | Realtek RTS525A PCI Express Card Reader |
| 键盘热键 | Dell WMI Hotkeys (Bus: 0x19) |

### BIOS版本

- **[1.36.0](https://www.dell.com/support/home/en-us/drivers/driversdetails?driverid=rv03k&oscode=biosa&productcode=latitude-14-7490-laptop)**

### Bootloader / OC EFI版本

- **[OpenCore 0.9.9](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.9)**

### SMBIOS型号

- **MacBookPro15,2**
- 基于[GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)生成的PlatformInfo信息

## BIOS设置

- Boot mode（启动模式）: UEFI
- Fast Boot（快速启动开关）: Thorough
- SecureBoot（安全启动）: Disable
- SATA Mode（SATA工作模式）: AHCI 
- Intel SGX: Software Controlled

## 哪些功能可以正常工作

- [x] 核显显示
- [x] 电源管理
- [x] 系统唤醒 / 睡眠 (电脑盖开合 + 热键Fn+Insert)
- [x] 屏幕背光
- [x] WiFi (2.4Ghz + 5Ghz)
- [x] 蓝牙（包括音频）
- [x] 触控板 + 手势 + 小蓝点 + 左右按钮
  - 启用触控板的**单指左键，双指右键**:
    `设置` → `触控板` → `轻点来点按`
- [x] 热键支持 (Fn+F2/F3调整音量，Fn+F11/F12或Fn+S/B调整屏幕亮度)
- [x] USB-C充电

## 哪些功能无法正常工作

- 内置扬声器 (需要调试**layout-id**使**`AppleALC`**正常工作)
- 有线网卡 (需要调试IntelMausi.kext)
- 雷电接口 (已知bug，暂无修复计划)
- Handoff（接力）, Airdrop（隔空投送） & Sidecar（随航） (需要替换成博通的无线网卡)

## 哪些功能未经测试

- [ ] 二合一3.5mm耳机孔
- [ ] CPU频点步进
- [ ] 核显加速
- [ ] 内置麦克风
- [ ] HDMI输出 + HDMI音频输出
- [ ] 前置摄像头
- [ ] USB 3.0
- [ ] MicroSD读卡器 (手头没有SD卡)
- [ ] USB-C DP-alt Mode
- [ ] USB-C数据传输
- [ ] FileVault 2
- [ ] 指纹传感器 (无硬件，未标配)
- [ ] 智能读卡器 (无硬件，未标配)
- [ ] WWAN 4G卡 (无硬件，未标配)

## 特别感谢

- [CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh](https://github.com/CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh) **(主要参考)**

## Enjoy!

- 如何有任何bug（**最好是已知的修复手段**），欢迎**随时（尽快）联系我**，感激不尽

