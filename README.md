# FreeBSDpi

## Prerequisites

[FreeBSD ARM](https://mirror.herrbischoff.com/freebsd/releases/ISO-IMAGES/11.0/FreeBSD-11.0-RELEASE-arm-armv6-RPI2.img.xz) installed on a Micro SD card.

```sh
cd /usr/ports/ports-mgmt/portmaster/
make install clean

portmaster devel/ccache
portmaster ftp/curl
```

## Install Ports Collection

```sh
portsnap fetch extract
```

## Get System Source Code

```sh
curl -s https://mirror.herrbischoff.com/freebsd/development/tarballs/src_stable_11.tar.gz | tar xfv - -C /usr
```
