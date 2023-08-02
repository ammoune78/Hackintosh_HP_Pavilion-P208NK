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
- nVIDIA GeForce 840m
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
- nVIDIA GeForce 840m *
- Original Wireless card needs to be replaced *


## Instructions:
This EFI, is purely minimalist in therms of config used options, this will keeps macOS in a more stable state. In addition, the ACPI battery code wasn't used, which needs much more ACPI renames & code deletes with a new battery table patch under EC Device that needs to be added. This is very careful for HP Inside Bios, that doesn't like does kind of tweakings, to prevent it from possible corruption: the Battery is the best exemple as of possible corruption under windows & other OS's is expected. But, a kext is now is used to manage Battery Level & Charging, including the AC Power Adapter. The conclusion: "The cleanest means The stable".

The OpenCore version used is the 0.9.3, and you'll find in the releases section, every opencore version that ive added to this repository. You'll have to generate your own credible serials, add your proper Wireless Kexts as far as you swap your original WiFi card with another one.
Keep in mind, that if you're using this build for another similar HP laptop, with the same Intel CPU generation (Broadwell), you'll have to generate your own CPUFriendData kernel extension to lower the CPU frequency, otherwise the frequency will remain over the 1,20 GHz.

Last and not least, for better display comfort, i'll recomand you changing the LCD panel with FHD 1920 * 1080. This will let you enjoy your laptop more on every OS, not only APPLE's one.


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
  > - tonymacx86 for "charlatanism things", yes, i'll never! But, i give a thanks to users on their website here: ## FormerUser-435514 
- vit9696 and The HermitCrabs Lab.
- CorpNewt
- Laura Müller (Mieze)
- [FormerUser-435514]([url](https://www.tonymacx86.com/threads/guide-hp-pavilion-15-ab216tx-catalina-using-opencore.285539/)) for his guid, who helped me a lot in thinking that my laptop is able to receive macOS installation.
- [dkoluris]([url](https://github.com/dkoluris/HP-PROBOOK-470-G2-OpenCore)) for using a simple and clean EFI folder without ACPI altering, and only using ECEnabler for battery management & infos


## My bad salutation to TonyMacX86
> - You have a lot of bad track records with me and, especially for banning users who did nothing wrong, bad or things prohibited, following your policy that you don't follow in every aspect. I'm not the first banned, and sertennely not the last one, but i use these words to prevent people, who aren't conscious of your Darkest and Impostor devilous, charlatan step:
> - The beginning was, after posting a patch request for my GA-Z87X-UD4H, you stopped me from entering that Thread. Months after posting my patch for this board at InsanelyMac, pjalm attaqued me there, because i posted my patch, which was build by me. The attack then, has been rejected by the site owner, after examining all my code, which by the way, was having better code than pjalm's one.
> - Months after, pjalm posted my patch for the GA-Z87X-UD4H in the GIGABYTE MaciASL patch repository, and adding it also to the other GIGABYTE Z87 series MaciASL patch repository, thing that wasn't there at the moment of my request and before i posted my patch. This was ridiculous after seing it, and without a shame posting my patch without my consent.
> - years after, i requested from rehabman, who was the master piece on that website "keeping it alive in life" a solution for my previous pavilion core2duo laptop. Months after i posted a complete patch for that laptop, requesting rehabman adding it into his repository, thing that hasn't been done.
> - years after, the past two months, i posted a request for this laptop "Pavilion P208NK", minutes after, the post was deleted. I posted then, (Why i can't see my post?), then this second post has been deleted, wow, nice! I then posted the same first request, thinking that i didn't saved the comments before, then the TOP THING WAS MADE, they banned me for cause "?", really i don't know from the beginning!!!!!


## Who are TonyMacx86? Take a look by yourself here:
> - [Why InsanelyMac does not support tonymacx86](https://www.insanelymac.com/forum/topic/279450-why-insanelymac-does-not-support-tonymacx86/)
> - [I got banned on tonyMacx86, what do I do?](https://www.insanelymac.com/forum/topic/316980-i-got-banned-on-tonymacx86-what-do-i-do/)
> - [Tonymacx86-stance](https://github.com/khronokernel/Tonymacx86-stance)
