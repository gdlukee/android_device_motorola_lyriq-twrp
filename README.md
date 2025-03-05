# TWRP Device Tree for Motorola Edge 40 (lyriq)

## Status
### HEAVY WIP ⚠ NOT READY FOR USE

### Current feature checks:
- [ ] Correct screen/recovery size
- [ ] Working touch, display
- [ ] Backup/restore to/from internal/external storage
- [ ] ADB (including sideload)
- [X] Fastboot
- [ ] MTP
- [ ] Flashing zip/images

- [ ] All important partitions listed in wipe/mount/backup lists
- [ ] F2FS/EXT4 Support, exFAT/NTFS when supported
- [ ] Reboot to system
- [ ] Reboot to recovery
- [X] Reboot to fastboot
- [ ] Reboot to bootloader
- [X] Screen goes off and on
- [ ] Poweroff
- [X] Correct UI Colors

- [ ] Input devices via USB-OTG
- [ ] USB mass storage export
- [ ] Correct date
- [ ] Battery level
- [ ] Temperature
- [ ] Set brightness
- [ ] Vibrate and set vibration
- [X] Screenshot
- [ ] Advanced features

# Building
```bash
export ALLOW_MISSING_DEPENDENCIES=true
source build/envsetup.sh
lunch twrp_lyriq-eng
mka recoveryimage -j$(nproc --all)
```

**Copyright (C) 2025 Team Win Recovery Project**
