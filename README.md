# Hackintosh_HP_Pavilion-P208NK

# Install up to macOS Catalina in your Pavilion P208NK, just like a MacBook Pro 12,1!

## Overview:

In this repos, you'll have a complete EFI folder, that will let you install up to macOS Catalina, on this laptop.
OpenCore is the Bootloader used for this config, and is the best choice for this particular laptop, which won't let the macOS drive, be the first from the UEFI Boot Menu. The Windows drive will always remain the first, and will never result in a corrupted EFI folder. Thus, you will have to select the macOS drive on each reboot or power on, this is due to the HP Inside BIOS crap.

This laptop can let you install 3 drive in the same time:
1- The Original Drive
2- Swapping the Optical Drive with Caddy
3- M.2 Slot on the down side of the motherboard.

## Laptop Specifications:
- Intel core i7-5770
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
Acidanthera's Life's Easier for us: [Here]([url](https://github.com/acidanthera))
OpenCore: [Here]([url](https://github.com/acidanthera/OpenCorePkg))
Python: [Here]([url](https://www.python.org/downloads/))
CorpNewt's Life's Easier for us: [Here]([url](https://github.com/corpnewt))
ProperTree: [Here]([url](https://github.com/corpnewt/ProperTree))
GenSMBIOS: [Here]([url](https://github.com/corpnewt/GenSMBIOS))
gibMacOS: [Here]([url](https://github.com/corpnewt/gibMacOS))
One-Key-CPUFriend: [Here]([url](https://github.com/stevezhengshiqi/one-key-cpufriend))
ECEnabler Kext (Battery Infos): [Here]([url](https://github.com/1Revenger1/ECEnabler))

## Special Thanks
- Every Hackintosh Community: Specially InsanelyMac, Olarila, AppleLife.ru, Hackintosh-Montreal.com, Hackintosh-Forum.de, Hackintosh-Inc.de and many, but never tonymacx86 for "charlatanism things" no never! 
- vit9696 and The HermitCrabs Lab.
- CorpNewt
- Laura Müller (Mieze)
- [FormerUser-435514]([url](https://www.tonymacx86.com/threads/guide-hp-pavilion-15-ab216tx-catalina-using-opencore.285539/)) for his guid, who helped me a lot in thinking that my laptop is able to receive macOS installation.
- [dkoluris]([url](https://github.com/dkoluris/HP-PROBOOK-470-G2-OpenCore)) for using a simple and clean EFI folder without ACPI altering, and only using ECEnabler for battery management & infos

## My bad salutation to TonyMacX86
- you have a lot of bad track records, especially banning users for doing nothing wrong, bad, things prohibited by your policy that you don't follow in every aspect. I'm not the first banned, and sertennely not the last one. And i use these words to prevent people from your Dark and impostor devilous step. 
