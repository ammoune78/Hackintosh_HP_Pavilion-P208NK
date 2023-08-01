# Hackintosh_HP_Pavilion-P208NK

![HP-Pavilion_P208NK](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/133e37a6-b11b-4146-9b4d-8e3f08e09b39)


## Overview:

In this repos, you'll have a complete EFI folder, that will let you install up to macOS Catalina, on this laptop.
OpenCore is the Bootloader used for this config, and is the best choice for this particular laptop, which won't let the macOS drive, be the first from the UEFI Boot Menu. The Windows drive will always remain the first, and will never result in a corrupted EFI folder. Thus, you will have to select the macOS drive on each reboot or power on, this is due to the HP Inside BIOS crap.

This laptop can let you install 3 drive in the same time:
1- The Original Drive
2- Swapping the Optical Drive with Caddy
3- M.2 Slot on the down side of the motherboard.

## [Laptop Specifications](https://support.hp.com/ca-fr/document/c04536807):
- Intel core i7-5500u
- Intel 5500 HD Graphics
- nVIDIA GeForce 820m
- 1366 x 768 LCD Panel
- 8 GB SamSung RAM DDR3 1600MHz
- 1 TB Toshiba Hard Drive Disk
- Realtek ALC290 Audio Controller
- Realtek RTL8106EUS Ethernet Controller
- Broadcom Wireless Card (Not Compatible with macOS, and don't expect it to work! You need to buy a compatible one)
- Realtek SD-Card
- 2x USB 3.0 including one operating in backward compatibility & 1x USB 2.0
- Mouse & Trackpad fully working on macOS including gestures

# Screenshots Refence:

## About

![About](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/93e863e6-222f-4b5b-a009-eb481b523a6e)

## Audio

![Audio](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/e41081ab-f2d6-489c-a2b5-121d8e1807dd)

## Camera

![Camera](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/330b532c-d78c-4372-b778-cabd7d2ea6fc)

## Ethernet

![Ethernet](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/c70d1e00-916a-41c7-8942-b047df4b4a49)

## Graphics

![Graphics](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/739b761d-394f-442f-a05a-f5213a86a819)

## PCI

![PCI](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/3c5af9ac-2e75-4d2d-9ef1-e49e4f938c58)

## Power

![Power](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/efc745f9-d2eb-48e7-b7ef-8ce9274e2216)

## SATA

![SATA](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/979cec03-7825-4065-9e6d-4872abaec20a)

## USB

![USB](https://github.com/ammoune78/Hackintosh_HP_Pavilion-P208NK/assets/6939542/fdb3e3af-2ac4-4d82-a35a-fccd7f17eee2)



## What Works:
- Everything (*x 2)

## What doesn't works:
- nVIDIA GeForce 820m *
- Wireless card needs to be replaced *

## Instructions:
This EFI is purely minimalist in therms of config used options, including ACPI battery code that wasn't used, to don't alter UEFI firmware. A kext is now used to manage Battery Level & Charging including the AC Power Adapter.
The OpenCore version used is the 0.9.3, and you'll find in the releases section, every opencore version that ive added to this repository. You'll have to generate your own credible serials, add your proper Wireless Kexts as far as you swap your WiFi card with another one.
Kee in ming that if you're using this build for another similar HP lapto with the same Intel CPU generation (Broadwell), you'll have to generate your own CPUFriendData kernel extension to lower the CPU frequency, otherwise the frequency will remain over the 1,20 GHz.
For better display comfort, i'll recomand you changing the LCD panel with FHD 1920 * 1080. This will let you enjoy your laptop more on every OS, not only APPLE's one.

## Things that you may need:
- Acidanthera's Life's Easier for us: [Here](https://github.com/acidanthera).
- OpenCore: [Here](https://github.com/acidanthera/OpenCorePkg).
- Python: [Here](https://www.python.org/downloads/).
- CorpNewt's Life's Easier for us: [Here](https://github.com/corpnewt).
- ProperTree: [Here](https://github.com/corpnewt/ProperTree).
- GenSMBIOS: [Here](https://github.com/corpnewt/GenSMBIOS).
- gibMacOS: [Here](https://github.com/corpnewt/gibMacOS).
- One-Key-CPUFriend: [Here](https://github.com/stevezhengshiqi/one-key-cpufriend).
- ECEnabler Kext (Battery Infos): [Here](https://github.com/1Revenger1/ECEnabler).

## Special Thanks
- Every Hackintosh Community: Specially InsanelyMac, Olarila, AppleLife.ru, Hackintosh-Montreal.com, Hackintosh-Forum.de, Hackintosh-Inc.de and many, but never:
  > tonymacx86 for "charlatanism things" no never! 
- vit9696 and The HermitCrabs Lab.
- CorpNewt
- Laura Müller (Mieze)
- [FormerUser-435514]([url](https://www.tonymacx86.com/threads/guide-hp-pavilion-15-ab216tx-catalina-using-opencore.285539/)) for his guid, who helped me a lot in thinking that my laptop is able to receive macOS installation.
- [dkoluris]([url](https://github.com/dkoluris/HP-PROBOOK-470-G2-OpenCore)) for using a simple and clean EFI folder without ACPI altering, and only using ECEnabler for battery management & infos

## My bad salutation to TonyMacX86
> - you have a lot of bad track records, especially banning users for doing nothing wrong, bad, things prohibited by your policy that you don't follow in every aspect. I'm not the first banned, and sertennely not the last one. And i use these words to prevent people from your Dark and impostor devilous step. 
