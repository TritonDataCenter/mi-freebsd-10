# mi-freebsd-10

This repo allows one to create a custom ISO with the necessary packages and
tooling for deploying on SmartOS and Joyent Public Cloud.

## Requirements

This must be run on a FreeBSD machine or VirtualMachine.

## Setup

Before using mi-freebsd-10, please install the following packages:

```
pkg install -y bash rsync cdrtools git
```

## Usage

To build a custom ISO, run the `build_freebsd_iso` script:


```
./build_freebsd_iso
```

This will download an ISO, created a customized layout with installerconfig, then build the custom ISO.


## Customizing
You can modify the following if you'd prefer a different ISO, architexture, or FreeBSD mirror:

```
MIRROR="ftp.freebsd.org"
MIRROR_PATH="pub/FreeBSD/releases/amd64/amd64/ISO-IMAGES"
ISO="FreeBSD-10.1-RELEASE-amd64-disc1.iso"
CUSTOM_ISO_FILENAME="freebsd-10-custom.iso"
```
