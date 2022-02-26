## Alternative Halium installer script

> Hack by Flytreels  

The difference to the official script from the halium-scripts repository is that this script will prepare the rootfs on your host system instead of on the device. This will make you independent of problems like old TWRP images, no busybox or not-working busyboxes on some devices.

A prebuilt standalone version available [here](https://github.com/JBBgameich/halium-install/releases). Alternatively you can just clone this repository and directly use the script.

### Dependencies

* qemu-user-static
* e2fsprogs
* simg2img

### Usage:


Patch a halium rootfs and systemimage:
`halium-install -p <mode (reference, neon, ut, debian-pm, debian-pm-caf, none)> <rootfs.tar.gz> <system.img>`

### Standalone version
If you want to use this shell script independently of this folder, create a standalone script of it by executing `bash utils/standalone.sh`. You will find the executable in bin/halium-install-standalone.sh.
