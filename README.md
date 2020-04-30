# ThinkPad E580 EFI for Clover
## Based on the EFI Setup from github.com/dandepeched
Tested on 20KSA00SAU model with macOS Catalina (10.15.1)

### BIOS Settings
* I used BIOS version 1.40, it may work on lower versions too
* Disable Secure Boot

### What hardware doesnt work?
* Stock Wi-Fi Card (Intel AC 3165)
* Line/Mic Input (3,5")
* Card reader
* Cant use more than 3 fingers on the trackpad at once

### WiFi

As far as i am aware, the E580 does not have a wifi whitelist so you should be able to swap in a compatible wifi card.

### Post-Install

I recommend once you have installed macOS and copied over the EFI folder to the hard drives EFI partition that you randomise your UUID and serial number. You should also be able to remove `-v` from the boot args if it is booting stable.

**Note:** I was unable to format the built in nvme ssd as apfs without a kernel panic, your result may vary. i ended up having to fill the sata slot with a sata ssd and install onto that.

### You may run into other issues, you use this efi folder on your system at your own risk
