Cygnus
===========

Let's get started :)
--------------------
![Cygnus](Cygnus-06.jpg)

[![TG chat](https://img.shields.io/badge/Support-Telegram-%23e52c5f.svg?style=for-the-badge&logo=telegram&&labelColor=121217)](https://t.me/cygnusos)

To get started with Android/Cygnus, you'll need to get
familiar with [Repo](https://source.android.com/source/using-repo.html) and [Version Control with Git](https://source.android.com/source/version-control.html).


How to sync the source
```
repo init -u https://github.com/cygnus-rom/manifest.git -b caf-ten

repo sync -j$(nproc --all) --force-sync --no-tags --no-clone-bundle --prune --optimized-fetch
```



**COMPILING**


```
source build/envsetup.sh
lunch cygnus_devuce-userdebug
mka bacon -j$(nproc --all)
```

Contributing
-------------

Contributions through pull requests are welcome.


Credits
--------

- AOSP

