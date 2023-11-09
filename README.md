# EmptyIME
Keyboard with no UI. Used in automation and extracted as a standalone app from the Appium setting app.

Sometimes the adb command to change the IME fails. So when you need an empty keyboard with no UI. Use this app to set it during the emulator creation. More practical if you use docker. Just install, launch and enable the keyboard during the emulator localisation. Additionally, you  can docker-enter any prebuild docker images and install this app. Afterwards you can commit the modified image and use it.

### How to use
1. Install the apk from apk dir
2. Launch the app
3. Navigate to Settings >language> keyboard and enable the keyboard
4. To change the IME during automation use the below command
   
```bash
adb shell ime enable com.emptyime/.EmptyIME
adb shell ime set com.emptyime/.EmptyIME
```


