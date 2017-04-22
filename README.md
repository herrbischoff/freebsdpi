# FreeBSDpi

## Prerequisites

[FreeBSD ARM](https://mirror.herrbischoff.com/freebsd/releases/ISO-IMAGES/11.0/FreeBSD-11.0-RELEASE-arm-armv6-RPI2.img.xz) installed on a Micro SD card.

```bash
cd /usr/ports/ports-mgmt/portmaster/
make install clean

portmaster devel/ccache
portmaster ftp/curl
```
