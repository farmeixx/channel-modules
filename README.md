# channel-modules

Mainline kernel modules for the Motorola Moto G7 Play (channel / SDM632).

One module set that every distro rootfs builder (alpine, debian, ubuntu)
installs, so the rootfs no longer depends on per-run CI checkpoint
artifacts.

Layout mirrors the mainline kernel checkpoint:

- kernel-release.txt - kernel release string
- kernel-modules-<release>.tar.zst - the module set
- kernel.config - kernel configuration of the matching build
- System.map - symbol table of the matching build
- SHA256SUMS - checksums for everything above

Source: extracted from the validated alpine-20261031062555 rootfs
(mainline 7.3.0-rc7).
