# Raspbian Docker Container

[![][layers]][microbadger "Image Layers"]
[![][version]][microbadger "Image Version"]
[![][license]][microbadger"Image License"]
[![][commit]][github "Image Commit"]

Built daily so that the image has the latest [Raspbian][project] packages.

Available on Docker Hub as [vcatechnology/raspbian][docker-hub]

## Emulation

This Docker image can be ran on an x86_64 host. To do this, the
capability to run ARM executables transparently must be enabled. On Linux the easiest
way to do this is to install the `binfmt-support` package:

```
packagemanager install binfmt-support qemu-user-static binfmt-qemu-static
systemctl enable --now binfmt-support
```

[docker-hub]: https://hub.docker.com/r/vcatechnology/raspbian/
[project]: https://www.raspbian.org/
[github]: https://github.com/vcatechnology/docker-arch
[microbadger]: http://microbadger.com/images/vcatechnology/raspbian
[layers]: https://images.microbadger.com/badges/image/vcatechnology/raspbian.svg
[version]: https://images.microbadger.com/badges/version/vcatechnology/raspbian.svg
[license]: https://images.microbadger.com/badges/license/vcatechnology/raspbian.svg
[commit]: https://images.microbadger.com/badges/commit/vcatechnology/raspbian.svg
