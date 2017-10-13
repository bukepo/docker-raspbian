# Arch Linux Docker Container

[![](https://images.microbadger.com/badges/image/vcatechnology/raspbian.svg)](http://microbadger.com/images/vcatechnology/raspbian "Image Layers") [![](https://images.microbadger.com/badges/version/vcatechnology/raspbian.svg)](http://microbadger.com/images/vcatechnology/raspbian "Image Version") [![](https://images.microbadger.com/badges/license/vcatechnology/raspbian.svg)](https://microbadger.com/images/vcatechnology/raspbian "Image License")  [![](https://images.microbadger.com/badges/commit/vcatechnology/raspbian.svg)](https://github.com/vcatechnology/docker-arch "Image Commit")

Built daily so that the image has the latest [Raspbian](https://www.raspbian.org/) packages.

Available on Docker Hub as [vcatechnology/raspbian](https://hub.docker.com/r/vcatechnology/raspbian/)

This Docker image is intended to be ran on an x86_64 host. To do this the
capability to run ARM executables natively must be enabled. On Linux the easiest
way to do this is to install the `binfmt-support` package:

```
packagemanager install binfmt-support qemu-user-static
systemctl enable --now binfmt-support
update-binfmt --display
update-binfmt --enable qemu-arm
```
