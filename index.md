## Notes to myself

### Reset root password on RHEL 8

`rd break`

`mount -o remount,rw /sysroot`

`chroot /sysroot`

`passwd root`

`touch ./autorelabel`

### Upgrade Fedora firmware

`sudo fwupdmgr refresh`

`sudo fwupdmgr get-updates`

`sudo fwupdmgr get-devices`