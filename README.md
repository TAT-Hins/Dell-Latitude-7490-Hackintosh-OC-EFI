# Dell-Latitude-7490-Hackintosh-OpenCore-EFI

# **[English]()|[中文文档]()**

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
- Generated **PlatformInfo** based on [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

## BIOS Settings

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



## What's working

- [x] iGPU displaying

- [x] Battery Management

- [x] Wake / Sleep (Lid & Fn + Insert)

- [x] Screen backlight control

- [x] WiFi (2.4Ghz + 5Ghz)

- [x] Bluetooth (Including Audio, tested with **`HUAWEI FreeBuds 4`**)

- [x] Touchpad with Gestures + Trackpad + Buttons
  - Enable **Touchpad click button (single for left click / double for right click)**:
    
    > `System Settings` → `Trackpad` → `Tap to click` 
  
- [x] Native hotkeys support with Fn keys (Volume Fn+F2/F3 and Screen Brightness Fn + F11/F12)

- [x] Web Camera

- [x] Internal Speaker & Microphone （tested **layout-id=`17`**）

- [x] USB-C charging

- [x] USB-C Data transfer (Tested with **Portable Hard Drive** & **`Android File Transfer`**)

- [x] USB 3.0 (Cost about 3s for copying a 1.0GB file, **over 300MB/s**)

  - **`USB 3.1 Bus`** also noticeable in **System Report**

- [x] USB-C accessory (Tested with **`HUAWEI USB-C Headset`**)

- [x] MicroSD card reader

## What's not working

- Ethernet 
  - No more crash, recognized correctly in system as **`Intel I219LM4 PCI Express Gigabit Ethernet`**
  - The indicator lights go on for seconds, but then go off after connected to the router
  - In the system it shows "Not connected"

- 2-in-1 3.5mm headphone jack
- Thunderbolt 
  - Known issues → not planning to fix currently

- Handoff, Airdrop & Sidecar 
  - needs to replace a Broadcomm wireless adapter


## What's not tested yet

- [ ] CPU Speedstep
- [ ] iGPU acceleration
- [ ] HDMI + audio over HDMI
- [ ] USB-C DP-alt Mode
- [ ] FileVault 2
- [ ] Fingerprint sensor (No hardware, SKU not included)
- [ ] WWAN card (No hardware, SKU not included)


## Special credits

- [CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh](https://github.com/CloverLeafBG/Dell-Latitude-7490-OC-Hackintosh) **(Mostly as referenced)**


## Enjoy!

- Please **let me know ASAP** if there're any bugs that can be fixed
