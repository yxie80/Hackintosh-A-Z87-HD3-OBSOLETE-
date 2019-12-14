# Hackintosh
Joost's Hackintosh system (MacOS 10.15.2 on GA-Z87-HD3, i5 4670K and RX 570)

![alt test](/Pictures/AboutFinder.png)

- Attached screenshots of the settings in Clover Configurator
- Attached zip of EFI folder, which you can use if you have the same/similair system
- Updated succesfully from 10.15.1 to 10.15.2 with latest Kext files

# PC specifications:
- Processor: Intel Core i5 4670K Boxed (Haswell)
- Motherboard: Gigabyte GA-Z87-HD3
- Sound card (onboard): Realtek ALC892 audio chip
- SSD storage: Crucial Crucial MX500, 1TB 
- Graphic card: Sapphire Nitro+ Radeon RX 570 4GD5
- OS installed: Catalina 10.15.2 dualbooted with Windows 10

# Prerequisites:
-	Patience (this was hard for me)
-	Make sure your motherboard is on the latest available BIOS.
-	Make a Bootable USB stick (from a actual Mac) using this procedure:
https://www.tonymacx86.com/threads/how-to-create-a-macos-catalina-public-beta-installation-usb.278188/ 

# Notes:
- I didn’t do anything at all with the Library/Extensions folder myself (it has lots of files in in though). For kexts, I only used the EFI/CLOVER/kexts/Other/ folder.

# Kexts:
Make sure (!) you are using the latest kexts from the internet: 

- FakeSMC.kext (Only install FakeSMC.kext, nothing else)
https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/
- USBInjectAll.kext
https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/
- Lilu.kext
https://github.com/acidanthera/Lilu/releases
- WhateverGreen.kext
https://github.com/acidanthera/WhateverGreen/releases

# BIOS Settings (from tonymacx86.com):
- To access BIOS/UEFI Setup, press and hold Delete on a USB Keyboard while the system is booting up
- Load Optimized Defaults
- If your CPU supports VT-d, disable it
- If your system has CFG-Lock, disable it
- If your system has Secure Boot Mode, disable it
- Set OS Type to Other OS
- If your system has IO Serial Port, disable it
- Set XHCI Handoff to Enabled
- If you have a 6 series or x58 system with AWARD BIOS, disable USB 3.0
- Save and exit.

# Work Procedure:
- Step 1: 
After power on, press F12 to select bootable USB.
Just boot from the USB boot disk and install.
Be sure to insert the USB into the USB 2.0 port.
- Step 2: 
Install macOS Catalina on Any Supported Intel-based PC.
I have omitted the detailed steps above. Only thing you should do, is during the entire process, boot via the USB stick.
- Step 3 (perhaps this step is redundant to step 4, but I did it anyhow): 
After installation is complete, install Clover (Clover_v2.5k_r5100 by Dids), install Clover Configurator and update it first. After that, mount the EFI of the SSD with Clover Configurator.
- Step 4: 
Delete the EFI folder of the SSD (intel SSD) with Catalina installed and EFI.ZIP
Please paste and unzip. And extract it in your EFI folder.
- Step 5:
Start Kext Utility
Prepare the permissions.
- Step 6:
Restart
- Step 7: 
Select and start the SSD on which Catalina is installed on.
 
# Confirmed working
-	CPU, RAM, Fans, etc.
- Video
-	Ethernet
-	Sound

# Extras
- Hide unneeded volumes in Clover with Clover Configurator. I've hide the following volumes:

![alt test](/Pictures/HideVolumes.png)

# Resources
https://www.tonymacx86.com/resources/clover-configurator.429/ 
https://hackintosh.gitbook.io 
https://www.tonymacx86.com/threads/how-to-create-a-macos-catalina-public-beta-installation-usb.278188/
https://www.tonymacx86.com/threads/unibeast-install-macos-mojave-on-any-supported-intel-based-pc.259381/#uefi_settings
