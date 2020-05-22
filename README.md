# Cygnus


## Let's get started

![Cygnus](Cygnus-06.jpg)

[![TG chat](https://img.shields.io/badge/Support-Telegram-%23e52c5f.svg?style=for-the-badge&logo=telegram&&labelColor=121217)](https://t.me/cygnusos)

To get started with Android/Cygnus, you'll need to get
familiar with [Repo](https://source.android.com/source/using-repo.html) and [Version Control with Git](https://source.android.com/source/version-control.html).

**BUILD ENVIRONMENT**

Apart from the basic compiling setup, make sure you have git lfs installed in your system.

In Ubuntu, do : 
```
sudo apt install git-lfs
```

**INITIALISING THE MANIFEST**

```
repo init -u https://github.com/cygnus-rom/manifest.git -b caf-ten
```

**SYNCING THE SOURCE**

```
repo sync -j$(nproc --all) --force-sync --no-tags --no-clone-bundle --prune --optimized-fetch
```

**SYNCING GAPPS**
```
repo forall -c git lfs pull
```

**COMPILING**


```
source build/envsetup.sh
lunch cygnus_device-userdebug
mka cygnus
```

### Contributing

Contributions through pull requests are welcome.
Gerrit coming soon!

## Credits

- AOSP
- LineageOS
- AOSPA
- WaveOS
And all other sources which could not end up in this list as it would become very long.
