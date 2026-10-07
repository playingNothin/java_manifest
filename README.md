# java_manifest — Moto G20 (`java`) LineageOS 18.1 bring-up

Manifest for assembling the complete Android 11 / LineageOS 18.1 source tree
that builds the Moto G20 (`java`, Unisoc UMS512/sharkl5Pro) ROM.

## Sync

    repo init -u https://github.com/LineageOS/android.git -b lineage-18.1 --git-lfs
    mkdir -p .repo/local_manifests
    curl -o .repo/local_manifests/java.xml \
      https://raw.githubusercontent.com/playingNothin/java_manifest/master/java.xml
    repo sync -c -j8

## What it adds / replaces

Own device trees: device/motorola/java, vendor/motorola/java,
kernel/motorola/java, packages/apps/MotoActions.

Forks (LineageOS upstream + `java` bring-up commits): system/core, build/make,
frameworks/av, frameworks/opt/net/wifi, hardware/interfaces, system/sepolicy,
vendor/lineage, hardware/ril, external/boringssl,
prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9.

Everything else comes from the standard LineageOS 18.1 manifest.
