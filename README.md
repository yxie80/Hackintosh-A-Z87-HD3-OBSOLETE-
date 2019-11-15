# Hackintosh
Joost's Hackintosh system (MacOS 10.15.1 on GA-Z87-HD3, i5 4670K and RX 570)

# PC specifications:
- Processor: Intel Core i5 4670K Boxed (Haswell)
- Motherboard: Gigabyte GA-Z87-HD3
- Sound card (onboard): Realtek ALC892 audio chip
- SSD storage: Crucial Crucial MX500, 1TB 
- Graphic card: Sapphire Nitro+ Radeon RX 570 4GD5
- OS installed: Catalina 10.15.1 dualbooted with Windows 10

# Prerequisites:
-	Patience (this was hard for me)
-	Make sure your motherboard is on the latest available BIOS.
-	Make a Bootable USB stick (from a actual Mac) using this procedure:
https://www.tonymacx86.com/threads/how-to-create-a-macos-catalina-public-beta-installation-usb.278188/ 

# Notes:
I didn’t do anything at all with the Library/Extensions folder. For kexts, I only used the EFI/CLOVER/kexts/Other/ folder.

# Work Procedure:
- Step 1: 
After power on, press F12 to select bootable USB.
Just boot from the USB boot disk and install.
Be sure to insert the USB into the USB 2.0 port.
- Step 2: 
Install macOS Catalina on Any Supported Intel-based PC.
I have omitted the detailed steps above. Only thing you should do, is during the entire process, boot via the USB stick.
- Step 3 (perhaps this step is redundant to step 4, but I did it anyhow): 
After installation is complete, install Clover (Clover_V2.5k_r5098 by Dids), install Clover Configurator and update it first. After that, mount the EFI of the SSD with Clover Configurator.
- Step 4: 
Delete the EFI folder of the SSD (intel SSD) with Catalina installed and EFI.ZIP
Please paste and unzip. And extract it in your EFI folder.
- Step 5:
Start Kext Utility
Prepare the permissions.
- Step 6:
Restart
- Step 7: 
Select and start the SSD (intel SSD) which installed Catalina.
 
# Confirmed working
-	Video
-	Ethernet
-	Sound (with a customization for Stereo speakers and 1 Subwoofer) 
-	

# Resources
https://www.tonymacx86.com/resources/clover-configurator.429/ 
https://hackintosh.gitbook.io 
https://www.tonymacx86.com/threads/how-to-create-a-macos-catalina-public-beta-installation-usb.278188/
