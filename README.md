# XTLANDRIG
Stellite Cash (XTL) Android XMRIG. An android cpu miner. This is beta release of binaries compiled from stellitecoin/xtlandrig for public testing before original release version. Please contact us via discord https://discord.gg/DVPJ5uD for any issues. The fee will be 0% for miners for now this does not include pool fees.

## Pools
Below are pools that have low difficulty which is appropriate for mobile mining (less than 1000 difficulty).

| URL | Starting Difficulty |
|----------------------------------|---------------------|
| stratum.xtlpool.com:8888 | 1000 |
| dearmon.zone:8988 | 50 |
| xtl.pool.gntl.co.uk: | 1000 |
| stellite.almsoft.net:3333 | 1000 |
| xtl.superpools.online:33333 | 500 |
| Pool.XTL.CryptoPool.Space | 500 |
| communitypool.stellite.cash:6677 | 1000 |
| Mine.Stellite.Cash:80 | 500 |


## How to use

1. Download base on platform architechure. Currently support
 * arm64-v8a
 * armeabi-v7a
 
 2. Install adb. More info on adb and to install
 https://developer.android.com/studio/command-line/adb
 https://www.xda-developers.com/install-adb-windows-macos-linux/
 
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
    
    Execute the binary ```./xtlandrig -o <pool address> -u <xtl_address> -p x```
