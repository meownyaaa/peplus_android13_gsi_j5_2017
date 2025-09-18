# Notes

### [Bugs](#bugs)

### You need a vendor partition before starting. Check the [downloads](#downloads) for the creator.

### You also need a custom recovery, duh. Check [downloads](#downloads).


### It will take a while for the boot animation to appear, your phone most likely hasn't crashed.


### Set status bar top padding to 2, start padding to 30, and end padding to 0 to make it look even. You will need to enable dynamic superuser in Misc settings if you do not have Magisk/Dynamic Superuser.


### System UI will occasionally lag out and android will keep telling you it "isn't responding", the not responding thing is a bug and google still has not fixed it even in Android 16 (good ol' google), but the lagging out is not as you're running Android 13 with pixel features on 2 whole fucking gigabytes of RAM (assuming you didnt buy the 32gb J5 2017 which has 3GB RAM)


## !!! If you choose to use another vendor, if you don't set lock screen to none, it will cause a crash when it loads after rebooting and you will be unable to use the phone until you format data. (Unverified)

# HALF ASSED TUTORIAL IM LAZY TODAY

Boot into TWRP, push the vendor creator to /sdcard, flash the vendor creator.

Reboot back into TWRP, push the resizer of choice, flash and follow the instructions it gives you (Change filesystem in advanced wipe if unable to wipe normally, and use format data instead of advanced wipe)

Push the kernel and vendor to /sdcard, flash both zips.

Push the gsi to /sdcard, press "Install image" and select it, select System to be flashed to. If the GSI image doesn't appear, reboot into recovery again.

After that, wipe Internal storage to get rid of the files so you don't have to in Android.

**[Also, remember the notes. Do not set a screen lock in setup.](#you-must-not-set-a-screen-lock-in-setup-it-will-cause-it-to-crash-loop)**

# Downloads

[Ares 7.0 (SIMPLE KERNEL V2)](https://drive.google.com/drive/folders/10eb8C9UY8tuZGcFGr_gHCcce6oDsxOwp)

[Vendors for J5 2017/J6 2018 (Telegram channel)](https://t.me/j7_7870/158695)

[PE Plus GSI](https://github.com/ChonDoit/treble_peplus_patches/releases) (Choose the PE-Plus_A13-arm64-bgS-slim_XXXXXXXX.img.xz if you want dynamic superuser, bgN-slim if you dont)

[Partition resizer](https://xdaforums.com/t/tool-7870-universal-repartition-script-for-vendor-support.4143541) ---------- [3.5GB system version](https://github.com/meownyaaa/peplus_j5_2017_j6_2018/releases/download/1/universal7870_repartitioner_3.5gb_system.zip)

[Vendor creator (jXy17lte)](https://drive.google.com/drive/folders/1TfoongsPcP6JRL1pVoLbP9t3FYhnNZOr)

[TWRP for 7870](https://t.me/j7_7870/189741) ---------- [J5 2017 Odin TAR](https://github.com/meownyaaa/peplus_j5_2017_j6_2018/releases/download/2/FLASH.TO.AP.tar)

# Bugs

### The brightness will be broken because of X-Rom vendor, you can semi fix this by following the below video

https://github.com/user-attachments/assets/32446cc9-a620-4cde-b8b1-ac4c1646550d


### Hardware navigation buttons (home button, capacitive recents and back) do not work, most likely because of the vendor. Fingerprint works fine, though.


### Always-on display does not work properly if you force it to be enabled in the settings.


### Wi-Fi will disable itself every reboot, this is the vendors fault.


### You must NOT set a screen lock in setup, it will cause it to crash loop.
If you have set one by accident, adb is enabled by default. Connect your device to another device that can access adb and run `adb shell am start -a android.settings.SETTINGS`, then disable the screen lock in security.


## Credits
These people have helped this project in some way or another, so they should be the ones who receive all the credit:
- [phhusson](https://github.com/phhusson)
- [AndyYan](https://github.com/AndyCGYan)
- [ponces](https://github.com/ponces)
- [eremitein](https://github.com/eremitein)
- [Peter Cai](https://github.com/PeterCxy)
- [haridhayal11](https://github.com/haridhayal11)
- [Iceows](https://github.com/Iceows)
- [X-Rom for vendor](https://xdaforums.com/t/rom-s-j5-2017-j6-xrom-oneui-4.4612785)
- [Project_Spaget X for vendor creator](https://xdaforums.com/t/treble-arm64-aosp-j701x-project_spaget-x.3953463)
- [ChonDoit for GSI](https://github.com/ChonDoit)
- [7870 Telegram group for downloads](https://t.me/j7_7870)
