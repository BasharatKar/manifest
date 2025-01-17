![20220310_215258](https://user-images.githubusercontent.com/87426352/157710326-991ecb31-65cf-460b-b3ec-d6ddad1edbdb.png)
---------------------------------------------------------------------------------------
 Getting Started:
 ==============

To get started with Project Blaze, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To initialize your local repository, use a command like this:

```bash
repo init -u https://github.com/ProjectBlaze/manifest.git -b 12.1
```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune
```

---------------------------------------------------------------------------------------
 Compilation of ProjectBlaze:
 ==================

From root directory of Project, perform following commands in terminal

```bash
$ . build/envsetup.sh
$ lunch blaze_$device-userdebug
$ brunch <device_codename>
```
NOTE:
If building for your device, adapt your tree to our configurations. Use this [commit](https://github.com/ProjectBlaze-Devices/device_xiaomi_onclite/commit/4a4dee0f51f21bb3c45b8b9e77639b43ae0eb556) as a reference.
---------------------------------------------------------------------------------------
