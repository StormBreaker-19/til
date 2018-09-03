# Flashing Android

1. `brew cask install android-platform-tools` (don't need the whole Android SDK) 

2. Download latest image: https://developer.android.com/preview/download.html and unzip. 

3. Enable Developer Mode (tap build number 5 times) and turn on 'OEM Unlocking' and 'USB Debugging' and plug in. 

4. `adb devices` to check it’s connected 

5. `adb reboot bootloader` 

6. `fastboot flashing unlock` 

7. `fastboot reboot-bootloader` to be safe 

8. `fastboot devices` to check it’s still connected 

9. `fastboot flash bootloader [bootloader file].img` 

10. `fastboot reboot-bootloader` 

11. `fastboot flash radio [radio file].img` 

12. `fastboot reboot-bootloader` 

13. `fastboot -w update [image file].zip` 

14. Start phone up. Skip everything. 

15. Enable Developer Mode, again. 

16. `fastboot flashing lock` to relock the bootloader (required for Google Pay)
