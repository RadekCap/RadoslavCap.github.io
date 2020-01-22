### LVM

#### Prepare
`parted -set NUMBER lvm on`

`pvcreate ...`

`vgcreate ...`

`lgcreate ...`

`mkfs.xfs /dev/.../lv`

#### Manage

`vgextend vg_name /dev/...`

`lvextend ...`

`xfs_growfs /mnt_point`


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