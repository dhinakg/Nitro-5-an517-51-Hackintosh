## Nitro-5-an517-51-Hackintosh

![](/images/main1.png)
![](/images/File1.png)
![](/images/File2.png)
# Files are always updated

Supports MacOS 10.15.x, **tested only on catalina but it should work on (10.14.x and 10.13.x)**

##### What's Working...
* Sleep (https://laptop.dortania.ml/battery-power-management/correcting-sleep-problems.html) (Disabling Hibernation)
* Power Managment is very stable most of the time cpu Fan will not load but it depends on what you are doing
* TouchPad + all gestures Finally after month of researching
* Fully Functional QE/CI Enabled Graphics
* Display brightness with hot keys
* FaceTime, Messages, etc...
* iGPU with disabled dGPU
* Audio & headphone jack
* Battery Management
* All USB ports
* WebCam
* Ethernet
* Sidecar


##### Disabled Devices
* Bluetooth
* GTX 1660Ti
##### BIOS Settings

* Security → Set supervisor password (to disable secure boot)
* Security → Password on boot → Disable
* Boot → Secure Boot → Disable
* Main → click on (calt+s) a new setting will appear to change SATA type to AHCI otherwise you will not be able to see you drive when installing  hackintosh
 # WIP
 ####  Bios Unlock to unlock CFG and have full control over your laptop (done without programmer)
 https://www.amazon.de/-/en/KeeYees-SOIC8-EEPROM-CH341A-Programmer/dp/B07SNTL5V6/ref=sr_1_2?dchild=1&keywords=ch341a&qid=1587467368&sr=8-2
 #### Wifi card replacment 
 https://www.amazon.de/-/en/gp/product/B081H6KZL8/ref=ppx_yo_dt_b_asin_image_o00_s00?ie=UTF8&psc=1
 
# Not Working
####  intel WiFi/Bluetooth not supported
####  HDMI (Nvidia Optimus is hardwire to HDMI)
# Important info 
#### when you switch SATA type to AHCI you might not be able to boot to windows again but do not worry here is a guide i found to switch without getting any issue https://support.thinkcritical.com/kb/articles/switch-windows-10-from-raid-ide-to-ahci
#### OpenCore Guide https://laptop.dortania.ml/

## Do not forget to generate new Smbios with clover configurator and for OC use GenSMBIOS (MacBook pro 16,1)
## &#x1F34F;  UPDATES 14.04.2020-OpenCore
* Add SSDT-USBX.aml for USB-Power because after i tested usb-stick 3.1 gen i noticed it did not worked so now all port work   normaly with super speed too 
* OC-Config.plist
## &#x1F34F;  UPDATES 12.04.2020-OpenCore
* Fix an issue when usb is pluged-in the laptop will not sleep with SSDT-GPRW 
* Replace SSDT-NoHybGfx with SSDT-NDGP_OFF to make sleep faster 
* OC-Config.plist

## &#x1F34F;  UPDATES 11.04.2020-OpenCore
* Replace DSDT with SSDT-BRKEY and SSDT-I2C-TPAD because placing DSDT will cause conflict with other patches
* Add NVMeFix.kext to get better power managment for NVMe
* OC-Config.plist

## &#x1F34F;  UPDATES 10.04.2020-OpenCore
* Brightness with native hot keys
* TouchPad has been fixed 
* OC-Config.plist
* ACPI Patches

## &#x1F34F;  UPDATES 07.04.2020-OpenCore
* better way to enable Apple ALC
* CPUFriend-1.2.0-DevBuild
* WhateverGreen-1.3.8
* Resources Folder
* VirtualSMC-1.1.2
* AppleALC-1.4.8
* OC-Config.plist
* Lilu-1.4.3


## &#x1F34F;  UPDATES 05.04.2020
* Add SystemProfilerMemoryFixup.kext to show memory section in about this Mac
* Add Theme to OpenCore Bootloader
* OC-Config.plist
* OpenCore 0.5.7
* Clover 5108
* Some missing parts :
* SSDT-DMAC
* SSDT-SBUS
* SSDT-XSPI
* SSDT-MCHC
* SSDT-PMC
* SSDT-MEM2
* SSDT-PPMC
* SSDT-SBUS-MCHC
* SSDT-HPET.aml

## Bios Version 
1.28 https://www.acer.com/ac/en/US/content/support-product/7966?b=1



