<div align="center">
<img src="https://files.catbox.moe/x7b0e2.png" height="128" width="128" style="border-radius:25%">
   <h1> Sepsemaphorin 
      <br/> 64-Bit Downgrade, Dualboot & Jailbreak Utility
   </h1>
</div>

<h4 align="center"> Uses seprmvr64 by mineek<h4>
<h6 align="center"> Supports iOS 7.0-12.5.7 as well as A7-A10x devices </h6>

# IF YOUR DEVICE SUPPORTS [LEGACY-IOS-KIT](https://github.com/LukeZGD/Legacy-iOS-Kit), YOU SHOULD REALLY USE THAT OVER THIS.

# Chart of device compatibility
all versions 7.0-12.5.7 are supported a7-a10x


# Chart of feature compatibility

| iOS         | App Store | Home button  | Volume keys | Cydia     | Tweaks  | Respring | Cellular | Sideloadly | iTunes |
|-------------|-----------|--------------|-------------|-----------|---------|----------|----------|------------|--------|
| 7.0.x**     | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|
| 7.1.x**     | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|
| 8.x**       | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|
| 9.x**       | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|
| 10.x**      | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|
| 11.x        | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|
| 12.x        | &#9745;   | &#9745;      | &#9745;     | &#9745;   | &#9745; | &#9745;  | &#9745;  | &#9745;    | &#9745;|

**recomed versions
## How do I use this?

This script deletes everything on your phone, including the main OS if you are not downgrading to iOS 10.3.3 or later. Make sure to backup all of your data before using this script as **anything on the device prior to running this script will be UNRECOVERABLE afterwards**. Use this script at your own risk. We are not responsible for any damages caused by you using this script.

To use this app, you need to downgrade to a supported version, and have a supported device.

`xcode-select install` to install `git` on macos

`git clone https://github.com/y08wilm/Semaphorin && cd Semaphorin`

Connect device in DFU mode

`sudo ./semaphorin.sh <the version you are downgrading to> --restore`

For example you may write `sudo ./semaphorin.sh 11.1 --restore`

The script has to backup important files from your current iOS version before you can downgrade.

When the script asks `[*] Please enter the iOS version that is currently installed on your device.`, type your current iOS version and then hit the Enter key to continue.

It should then begin the process of downgrading your device. Please follow the on screen instructions. This might take a while. Your device will reboot multiple times.

If you downgraded to iOS 9 or later, please use the jailbreak app on your home screen to begin jailbreaking your device.

## Subsequent runs after downgrade is finished

Connect device in DFU mode

`sudo ./semaphorin.sh <the version you downgraded to previously> --boot`

For example, if you downgraded to iOS 11.1, you would run `sudo ./semaphorin.sh 11.1 --boot`.

It should just boot to your requested iOS version normally.

## Requirements

linux or mac

Stable internet connection. Please don't try using this with dial up...

At least 20GB of free space on your computer

USB Type-A port and Lightning cable. USB Type-C ports will **NOT** work with this script. If you're using a Mac that only has a USB-C port (such as 12" MacBooks, and late Intel MacBook Airs) a dongle/dock with a USB-A port should work just fine with a standard USB-A to Lightning cable.

Working iDevice: The script has to backup `apticket.der`, `sep-firmware.img4`, `Baseband`, and `keybags` from your device before you can downgrade to an older iOS version.

## Support

We now have a [Discord server](https://discord.gg/WQWDBBYJTb) where you can get help with this project.

If, for whatever reason, that invite link does not work, please contact [wilm271](https://t.me/wilm271) on Telegram.

The Discord server is strictly for Semaphorin support only. Please don't bring personal issues into our server.

## Setup.app bypass
this willdelete setup.app to bypass actvation

## Troubleshooting

   The script only officially works on macOS 10.15 or later and linux due to some limitations on the developer's end. You have to install one of those versions to use the script. Please do not ask us about this.

Windows support is not planned either, do not ask about this either.

   ### Cydia is absent (on iPads)
   iPads have uicache issues with most jailbreaking tools. To open Cydia, enter `cydia://` in Safari's address bar and press Enter.  

   ### wtfis.app is absent (on iPads)
   iPads have uicache issues with most jailbreaking tools. To open wtfis, enter `wtfis://` in Safari's address bar and press Enter.  
## Credits

- [PsychoTea](https://github.com/PsychoTea/) for [MeridianJB](https://github.com/PsychoTea/MeridianJB/) which we use for iOS 10.3.3 downgrades
- [coolstar](https://github.com/coolstar) for [Electra](https://www.coolstar.org/electra/) and [Chimera](https://chimera.coolstar.org/) jailbreaks which we use on iOS 11 and 12 downgrades
- [edwin170](https://github.com/edwin170) for a ton of help with fixing cell service, icloud, audio, 3d touch, gyroscope, microphone and other issues
- [johndoe123](https://twitter.com/iarchiveml) for the a7 ios 7 [downgrade guide](https://ios7.iarchive.app/downgrade/) which made this entire project possible
- [LukeZGD](https://github.com/LukeZGD/) for the updated [cydia.tar](https://github.com/LukeZGD/Legacy-iOS-Kit/raw/main/resources/jailbreak/freeze.tar) for jailbreaking older ios versions
- [TheRealClarity](https://github.com/TheRealClarity) for wtfis.app which we [repurposed](https://github.com/y08wilm/wtfis/blob/ios7/wtfis/ViewController.m#L27) to run [evasi0n7](https://ios.cfw.guide/installing-evasi0n7/) for sandbox patch on ios 7 to allow cydia substrate to not break apps
- [Nathan](https://github.com/verygenericname) for the ssh ramdisk and [iBoot64Patcher fork](https://github.com/verygenericname/iBoot64Patcher)
- [Mineek](https://github.com/mineek) for [seprmvr64](https://github.com/mineek/seprmvr64) and other patches. I want to give a very special thanks to [Mineek](https://github.com/mineek), if it werent for them this entire project would have not been possible. you are amazing and i appreciate all that you do, thank you so much
- [nyuszika7h](https://github.com/nyuszika7h) for the script to help get into DFU
- [tihmstar](https://github.com/tihmstar) for [pzb](https://github.com/tihmstar/partialZipBrowser)/original [iBoot64Patcher](https://github.com/tihmstar/iBoot64Patcher)/original [liboffsetfinder64](https://github.com/tihmstar/liboffsetfinder64)/[img4tool](https://github.com/tihmstar/img4tool)
- [Tom](https://github.com/guacaplushy) for a couple patches and bugfixes
- [xerub](https://github.com/xerub) for [img4lib](https://github.com/xerub/img4lib) and [restored_external](https://github.com/xerub/sshrd) in the ramdisk
- [Cryptic](https://github.com/Cryptiiiic) for [iBoot64Patcher](https://github.com/Cryptiiiic/iBoot64Patcher) fork, and [liboffsetfinder64](https://github.com/Cryptiiiic/liboffsetfinder64) fork
- [libimobiledevice](https://github.com/libimobiledevice) for several tools used in this project (irecovery, ideviceenterrecovery etc), and [nikias](https://github.com/nikias) for keeping it up to date
- [Nick Chan](https://github.com/asdfugil) general help with patches and iBoot payload stuff
- [Serena](https://github.com/SerenaKit) for helping with boot ramdisk.
- [planetbeing](https://github.com/planetbeing/) for dmg tool from [xpwn](https://github.com/planetbeing/xpwn)
- [exploit3dguy](https://github.com/exploit3dguy/) for [iPatcher](https://github.com/exploit3dguy/iPatcher) which is used for patching iBoot on ios 7
- [dora2-ios](https://github.com/dora2-iOS) for [iPwnder](https://iarchive.app/Download/ipwnder_macosx)
- [NyanSatan](https://github.com/NyanSatan) for [fixkeybag](https://github.com/NyanSatan/fixkeybag)
