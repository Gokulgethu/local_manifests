# Local Manifests for OnePlus 11R (`udon` / `CPH2487`)

This repository contains the local manifest XML configuration for building LineageOS / AOSP based ROMs on **Crave.io** or local build machines.

## How to Use

### 1. In your Crave or ROM build root:
```bash
# Clone local manifest into .repo/local_manifests
git clone https://github.com/Gokulgethu/local_manifests.git .repo/local_manifests

# Sync all trees
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### 2. Build Commands (Crave / Server):
```bash
source build/envsetup.sh
lunch lineage_udon-userdebug
mka bacon
```
