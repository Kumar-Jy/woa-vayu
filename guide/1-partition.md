<img align="right" src="https://github.com/n00b69/woa-vayu/blob/main/vayu.png" width="350" alt="Windows 11 running on a Poco X3 Pro">

# Running Windows on the POCO X3 Pro

## Partitioning your device

### Prerequisites
- A brain

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

- [Modified TWRP](https://github.com/n00b69/woa-vayu/releases/tag/Recovery)

### Notes
> [!WARNING]  
> All your data will be erased! Back up now if needed.
> 
> Do not run the same command twice.
> 
> DO NOT REBOOT YOUR PHONE if you think you made a mistake, ask for help in the [Telegram chat](https://t.me/winonvayualt).
> 
> Do not run all commands at once, execute them in order!

> [!IMPORTANT]
> Make sure you use the MODDED Recovery throughout this whole tutorial as we provide tools to help aid this installation process and make it as easy as possible for you.
> 
> If you don't use it and you face any errors, consider it your fault and consider yourself alone if you try asking for support as you have deferred from the main guide.

### Opening CMD as an admin
> Download **platform-tools** and extract the folder somewhere, then open CMD as an admin.
>
> Replace **path\to** with the actual path to the platform-tools folder, for example **C:\platform-tools**
```cmd
cd path\to\platform-tools
```

#### Flash the modded recovery
> Replace **path\to** with the actual path to the modded recovery image
```cmd
fastboot flash recovery path\to\moddedtwrp.img reboot recovery
```

#### Run the partitioning script
> Replace **$** with the amount of storage you want Windows to have (do not add GB, just write the number)
> 
> If it asks you to run it once again, do so
```cmd
adb shell partition $
```

### Check if Android still starts
Just restart the phone, and see if Android still works

## [Next step: Installing Windows](/guide/2-install.md)














