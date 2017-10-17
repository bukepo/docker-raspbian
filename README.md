# Raspbian Docker Container

[![][layers]][microbadger] [![][version]][microbadger] [![][license]][microbadger] [![][commit]][github]

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

[docker-hub]: https://hub.docker.com/r/vcatechnology/raspbian/ "Docker Hub"
[project]: https://www.raspbian.org/ "Project"
[github]: https://github.com/vcatechnology/docker-arch "GitHub"
[microbadger]: http://microbadger.com/images/vcatechnology/raspbian "Microbadger"
[layers]: https://images.microbadger.com/badges/image/vcatechnology/raspbian.svg "Image Layers"
[version]: https://images.microbadger.com/badges/version/vcatechnology/raspbian.svg "Image Version"
[license]: https://images.microbadger.com/badges/license/vcatechnology/raspbian.svg "Image License"
[commit]: https://images.microbadger.com/badges/commit/vcatechnology/raspbian.svg "Image Commit"
