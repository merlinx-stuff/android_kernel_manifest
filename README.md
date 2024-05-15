## Repo Init ##
```bash
repo init -u https://github.com/merlinx-stuff/android_kernel_manifest.git -b android-mtk-mt6768-4.14-android11
```

## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Building Kernel ##

# For Merlinx
```bash
BUILD_CONFIG=kernel/xiaomi/mt6768/build.config.merlin build/build.sh
```

# For lancelot use
```bash
BUILD_CONFIG=kernel/xiaomi/mt6768/build.config.lancelot build/build.sh
```

## credit to Statixos for manifest