# Nekumori MOD
Xposed module. A collection of fixes for some apps to work properly, especially on OnePlus7.

## Fixes
- Rakuten Edy
```
The Rakuten Edy can work on a device without NFC-F, however it's not well tested. 
To use the app on an unsupported device, we need to bypass the device checking.
We spoof one of the supported device, Nexus 6 here. For more info, refer:
https://edy.rakuten.co.jp/howto/android/nfc/support/
```

- Google Daydream
```
NOTE: VR apps should be added to the LSPosed's scope for it to work.
(Ver 1.3) A new approach to enable Daydream using Xposed Framework.
Yep, there is no need to install another Magisk module! It works!
```
![](https://github.com/jeffshee/nekumori-mod/blob/master/images/daydream_vr.jpg)
```
(Ver 1.2) With Magisk Pix3lify module, we can get Daydream VR support on unsupported device.
Almost everything work, however, the main scene of Daydream app is visually distorted for unknown reason.
Issue on Pix3lify:
https://github.com/Magisk-Modules-Repo/Pix3lify/issues/104
And if we spoof Pixel device here, the distortion bug disappear, very weird indeed...
(Tested on OnePlus7, not sure if this can solve the same bug on different device)
```
_Before_
![](https://github.com/jeffshee/nekumori-mod/blob/master/images/daydream.jpg)
_After_
![](https://github.com/jeffshee/nekumori-mod/blob/master/images/daydream_fixed.jpg)

- Japan Post Bank
```
USB debug mode bypass for Japan Post Bank app.
```

- Remove Lock Screen Album Art (OxygenOS 10)

![](https://github.com/jeffshee/nekumori-mod/blob/master/images/album_art_removed_a10.jpg)
- Remove Lock Screen Album Art (OxygenOS 11)
```
OnePlus added the sh*t functionality back to the OxygenOS 11?
Don't worry, I got your back!
```
![](https://github.com/jeffshee/nekumori-mod/blob/master/images/album_art_removed_a11.jpg)

- Disable the stupid "Device supports Qualcomm® aptX™" notification

![](https://github.com/jeffshee/nekumori-mod/blob/master/images/aptx_notification.jpg)

- Hide "Clear All" button in Overview (Recent Screen)
```
NOTE: This mod is NOT enabled by default.
User who need this feature should opt-in by adding "OnePlus Launcher" to the LSPosed's scope.
```
![](https://github.com/jeffshee/nekumori-mod/blob/master/images/disable_overview_clear_all.jpg)

This mod aims to eliminate the bad habit of users who frequently press on the Clear All button for no reason.  
[Why it is a bad habit?](https://www.reddit.com/r/Android/comments/2gif4g/greenify_developer_says_constantly_swiping_away/) 