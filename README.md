# XTLANDRIG
Stellite Cash (XTL) Android XMRIG. An android cpu miner

## How to use

1. Download base on platform architechure. Currently support
 * arm64-v8a
 * armeabi-v7a
 
 2. Install adb. More info on adb https://developer.android.com/studio/command-line/adb
 
 3. Once you have adb installed and your android plugged onto your computer. Check if your device is connected. You can list connected devices by 
 ```
 adb devices
 ```
 
 3. By using adb put your selected xtlandrig binary into /data/local/tmp. You can do so as below
```
adb push xtlandrig /data/local/tmp/xtlandrig
```

 4. Next execute the binary on your device. To do this you have to go to shell mode by 
 ```
 adb shell
 ```
 
 5. In shell mode go to your binary placed location ```cd /data/local/tmp``` and execute ```./xtlandrig --help```. If you see the menu then your miner is ready.
 
 6. Running the binary requires 3 major things. 
    * Pool
    * XTL Address
    * Password
    
    Execute the binary ```./xtlandrig -o stratum+tcp://stratum.xtlpool.com -u <xtl_address> -p x```
