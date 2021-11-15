# `expand_rootfs`

This script can be run on a device that has been booted with a
volume (typically an SD card) created from a minimized image
(e.g. created by `sd2img`)

It will resize the root partition mounted at `/` to the maximum
size possible on the volume. In order to do so the root partition
must be the last partition on the volume / SD card.

IMPORTANT: As this script modifies a mounted partition / filesystem
it is crucial to reboot the machine immediately after running it to
ensure stable operation.