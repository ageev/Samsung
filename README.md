# Debloat Samsung S20 FE 5G or others 
On Phone:
1. Enable Developer Mode on the phone: ```Settings > About phone > Software information``` tap 10 times "Build number"
2. Go to ```Settings > (scroll to the bottom) > Developer options``` and enable "Wireless debugging"
3. In Wireless debugging menu click "pair device with paiting code". Note IP and Port (e.g. 10.0.0.10:65234) for pairing. Note! there are 2 sets of IP&Port - one for pairing, one for connect. 

on PC:
1. Download platform-tools https://developer.android.com/studio/releases/platform-tools to PC
2. Unpack and run ```adb pair [IP]:[Port]```. Use IP&Port for pairing! Type the pincode
3. ```adb connect [IP]:[Port]``` (use IP&Port for connect!)
4. ```adb shell```

to disable package run:
```pm uninstall -k --user 0 <package_name>```

to enbale run:
```pm install-existing --user 0 <package_name>```

See packages.txt in the repo for the list of bloatware

## Some noticable packages
```
com.sec.android.mimage.photoretouching  # Samsung photo editor
com.osp.app.signin # Samsung account sign in. Samsung account is needed for SmartThings
com.samsung.android.oneconnect # Samsung SmartThings
com.samsung.android.app.galaxyfinder # Slide bottom -> up menu
com.sec.android.app.soundalive  # needed for bluetooth headphones
com.samsung.android.dynamiclock  # nice dynamic wallpapers
com.samsung.android.themecenter # themes
com.samsung.android.lool # samsung Device Care (needed for scheduled reboots)
```
