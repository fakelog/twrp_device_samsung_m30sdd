# TWRP Device Tree for the Samsung Galaxy M30s

## How-to install dependencies
```
sudo apt install -y bison build-essential g++-multilib git make python zip openjdk-8-jdk repo screen libtinfo5 libncurses5
```

## How-to clone source and device tree:

```
mkdir -p ~/twrp && cd ~/twrp
```
```
repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0
```
```
repo sync
```
```
git clone https://github.com/fakelog/twrp_device_samsung_m30sdd.git device/samsung/m30sdd/
```
## How-to build:

```
export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch omni_m30sdd-eng; mka recoveryimage
```
Сompilation result is in ```twrp/out/target/product/m30sdd```
