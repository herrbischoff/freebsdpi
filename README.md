# FreeBSDpi

## Prerequisites

[FreeBSD ARM](https://download.freebsd.org/ftp/releases/arm/armv6/ISO-IMAGES/) installed on a Micro SD card.

### Install Ports Collection

```sh
portsnap fetch extract
```

### Set Make Options

Add everthing in [make.conf](etc/make.conf) to `/etc/make.conf`.

### Install Basic Tools

```sh
cd /usr/ports/ports-mgmt/portmaster/
make install clean

portmaster devel/ccache
portmaster ftp/curl
```

### Get System Source Code

```sh
curl -s https://mirror.herrbischoff.com/freebsd/development/tarballs/src_stable_11.tar.gz | tar xfv - -C /usr
```
