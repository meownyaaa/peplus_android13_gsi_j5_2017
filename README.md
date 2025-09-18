# Notes

You need a vendor partition before starting. Check the downloads for the creator.

You must NOT set a screen lock in setup, it will cause it to crash loop. 
If you have set one by accident, adb is enabled by default. Connect your device to another device that can access adb and run `adb shell am start -a android.settings.SETTINGS`, then disable the screen lock in security.

The brightness will be broken because of X-Rom vendor, you can semi fix this by following the video;
(to be made)

If you choose to use another vendor, the lock screen will cause a crash when it loads after rebooting and you will be unable to use the phone until you format data.

# Downloads

[Ares 7.0 (SIMPLE KERNEL V2)](https://drive.google.com/drive/folders/10eb8C9UY8tuZGcFGr_gHCcce6oDsxOwp)

[Vendors for J5 2017/J6 2018 (Telegram channel)](https://t.me/j7_7870/158695)

[PE Plus GSI](https://github.com/ChonDoit/treble_peplus_patches/releases) (Choose the bgS-slim_XXXXXXXX.img.xz GSI, I have not tested the bgN GSI)

[Partition resizer](https://xdaforums.com/t/tool-7870-universal-repartition-script-for-vendor-support.4143541) ---------- [3.5GB system version](https://github.com/meownyaaa/peplus_j5_2017_j6_2018/releases/download/1/universal7870_repartitioner_3.5gb_system.zip)

[Vendor creator (jXy17lte)](https://drive.google.com/drive/folders/1TfoongsPcP6JRL1pVoLbP9t3FYhnNZOr)

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
