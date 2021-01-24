# Cygnus


## Let's get started

![Cygnus](Cygnus-06.jpg)

[![TG chat](https://img.shields.io/badge/Support-Telegram-%23e52c5f.svg?style=for-the-badge&logo=telegram&&labelColor=121217)](https://t.me/cygnusos)

To get started with Android/Cygnus, you'll need to get
familiar with [Repo](https://source.android.com/source/using-repo.html) and [Version Control with Git](https://source.android.com/source/version-control.html).

**BUILD ENVIRONMENT**

**INITIALISING THE MANIFEST**

```
repo init -u https://github.com/cygnus-rom/manifest.git -b caf-11
```

**SYNCING THE SOURCE**

```
repo sync -j$(nproc --all) --force-sync --no-tags --no-clone-bundle --prune --optimized-fetch
```

**GAPPS**

Usage is highly recommended
```
WITH_GAPPS := true
```

**COMPILING**


```
source build/envsetup.sh
lunch cygnus_device-userdebug
make cygnus -j$(nproc --all)
```
## ADDITIONAL INFORMATION

Since Cygnus doesn't have pathmaps, you need to have your own HALs. You can take HALs from any ROM provided they build fine and don't have any pathmaps in them.
The paths for cloning HALs are as follows:

Audio -> ```vendor/qcom/opensource/audio-hal/primary-hal```

Media -> ```hardware/qcom/media```

Display -> ```hardware/qcom/display```

Of course, many HALs can be found in our devices org, on their respective caf-11-x branches and you can use them if your device has the same chipset, Happy Compiling!
### Contributing

Contributions through pull requests are welcome.

## Credits

- AOSP
- LineageOS
- AOSPA

And all others we might've missed out
