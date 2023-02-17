# Sync

```
repo init -u https://github.com/chrisl7/LA.UM.9.1.r1_manifest -b LA.UM.9.1.r1-12900-SMxxx0.0
```

```
repo sync -c -j$(nproc --all) --no-clone-bundle --no-tags --force-sync
```

# Build
```
 . build/envsetup.sh && lunch *-user && ./build.sh -j$(nproc --all) | tee log.xt
```