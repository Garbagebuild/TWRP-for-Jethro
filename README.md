# 📦 Custom TWRP Recovery for Jethro SC490

Welcome to the official TWRP recovery build for the **Jethro SC490** (SC490_MT6739).  
This custom recovery enables advanced Android maintenance features such as rooting, Nandroid backups, flashing custom zips, and more.

---

## ⚙️ Device Info

- **Model:** Jethro SC490  
- **Platform:** MediaTek MT6739  
- **Android Version:** 8.1 (Oreo)  
- **Architecture:** ARM32 (armeabi-v7a)

---

## 🔥 Features

✅ ADB & MTP enabled  
✅ Support for flashing ZIPs & images  
✅ Mount/unmount partitions  
✅ Terminal access  
✅ Backup & restore (NANDroid)  
✅ Built-in file manager  


---

## 📁 Files Included

- `recovery.img` – Custom TWRP recovery image (boot into this using fastboot or SP Flash Tool)
- (Optional) `MT6739_Android_scatter.txt` – SP Flash Tool scatter file if flashing via SPFT

---

## 🚨 Warning

> ⚠️ **Unlocking bootloader & flashing recovery can void your warranty and brick your device if done incorrectly.**  
> Proceed only if you understand the risks. Backup your data and **DO NOT** flash incorrect images or overwrite preloader/modem/tee unless you know what you’re doing.

---

## 🛠 Installation Guide

### 📲 ADB + Fastboot Method

1. **Enable Developer Options** and enable **OEM Unlocking** and **USB Debugging**  
2. Reboot to bootloader:
   adb reboot bootloader
   volume up...then volume down.
3. Flash TWRP:
   fastboot flash recovery recovery.img
   fastboot reboot
   adb reboot recovery.
   boots to recovery.  You have temporary root.

   PS:  The touch screen doesnt work but fortunately we still get adb root.  I have not confirmed OTG mouse works on this phone, although if you do confirm this, please post it in issues.
