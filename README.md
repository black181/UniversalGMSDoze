# Universal GMS Doze
*Prevent unnecessary GMS wakelocks running in the background, optimized & adjusted for better day to day battery life with additional modified services*

## Installation Guides
- API 23 or later is supported.
- Avoid to use similar modules or tweaks at once.
- Either install from Magisk Manager or any custom recoveries.

## Troubleshooting
- 60 seconds pause script for Magisk Boot Service.
- Does not guarantee for any modified Google apps (GApps) packages.
- Quick guide for how to fix delayed incoming messages issue, execute the script in terminal then reboot:
```
> su
> cd /data/data
> find . -type f -name '*gms*' -delete
```
- Checking optimization status for GMS in other way (outside from system Settings). Use any of your installed terminal app, do a simple execution script on below: (There's a line written `Whitelist (except idle) system apps:` and if this line `com.google.android.gms` does not exist it means that the module working fine and your GMS is optimized)
```
> su
> dumpsys deviceidle
```
- Force disable Find My Device if it is showing in Device administrators section. Use any of your installed terminal app, do a simple execution script on below:
```
> su
> pm disable com.google.android.gms/com.google.android.gms.mdm.receivers.MdmDeviceAdminReceiver
```

## Development Supports
- **Donations:**
  - BCA (Indonesia) 1390195385
  - [PayPal](https://paypal.me/gloeyisk)
- **Mirror Links:**
  - [Telegram Channel](https://t.me/GLdppc)
  - [SourceForge](https://sourceforge.net/projects/gldpsf/files/magisk_modules/)
- **Source Code:**
  - [GitHub](https://github.com/gloeyisk/UniversalGMSDoze)
- **Support Thread:**
  - [XDA-Developers](https://forum.xda-developers.com/apps/magisk/module-universal-gms-doze-t3853710)

## Credits
- **@topjohnwu**; [Magisk](https://github.com/topjohnwu/Magisk)
- **Contributors, Donators, Used/Needed Tools**
