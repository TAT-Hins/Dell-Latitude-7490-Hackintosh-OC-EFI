# Dell-Latitude-7490-Hackintosh-macOS-OpenCore-EFI


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

- **1.36.0**

### Bootloader

- **OpenCore 0.9.9**

### SMBIOS
- **MacBookPro15,2**


## BIOS Settings

- Boot mode: UEFI
- Fast Boot: Thorough
- SecureBoot: Disable
- SATA Mode: AHCI 
- Intel SGX: Software Controlled


## What's working

- [x] Battery Management

- [x] Sleep/Wake

- [x] WiFi (2.4Ghz + 5Ghz)

- [x] Bluetooth

- [x] Touchpad with Gestures + Trackpad + Buttons

- [x] Native hotkeys support with Fn keys (Volume Fn+F2/F3 and Screen Brightness Fn + F11/F12)

- [x] USB-C charging


## What's not working

- Fingerprint sensor

- Smart card reader

- Thunderbolt (needs to plug a device before boot)

- Handoff, Airdrop & Sidecar (needs to replace a Broadcomm wireless adapter)


## What's not tested yet

- [ ] CPU Speedstep

- [ ] iGPU acceleration

- [ ] Internal Speakers

- [ ] Internal Microphone

- [ ] Ethernet

- [ ] HDMI + audio over HDMI

- [ ] Web Camera

- [ ] USB 3.0

- [ ] MicroSD card reader 

- [ ] USB-C DP-alt Mode
 
- [ ] USB-C Data transfer

- [ ] FileVault 2

- [ ] WWAN card


## Special credits

- [CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh](https://github.com/CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh) **(Mostly as referenced)**


## Enjoy!

- Please **let me know ASAP** if there're any bugs that can be fixed

### 

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