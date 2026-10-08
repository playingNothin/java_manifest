# java_manifest

LineageOS 18.1 manifest for Motorola Moto G20 (`java`).

## Sync

    repo init -u https://github.com/LineageOS/android.git -b lineage-18.1 --git-lfs
    mkdir -p .repo/local_manifests
    curl -o .repo/local_manifests/java.xml \
      https://raw.githubusercontent.com/playingNothin/java_manifest/master/java.xml
    repo sync -c -j8

## Projects

Device:
- device/motorola/java
- vendor/motorola/java
- kernel/motorola/java
- packages/apps/MotoActions

Forks:
- system/core
- build/make
- frameworks/av
- frameworks/opt/net/wifi
- hardware/interfaces
- system/sepolicy
- vendor/lineage
- hardware/ril
- external/boringssl
- prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9

## Credits
FelipeCH: Testing the tree source
Motorola & Unisoc: Kernel Sources
