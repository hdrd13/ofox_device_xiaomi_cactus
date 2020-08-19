# device_xiaomi_cactus
## How to build TWRP from official repo?
1) mkdir twrp && cd twrp
2) repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0
3) repo sync
4) git clone https://github.com/recovery-xiaomi-mt6765/device_xiaomi_cactus -b master device/xiaomi/cactus
5) export ALLOW_MISSING_DEPENDENCIES=true
6) . build/envsetup.sh
7) lunch omni_cactus-eng
8) mka recoveryimage
### Out file twrp/out/target/product/cactus/recovery.img
