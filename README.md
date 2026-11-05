# GlassineOS/bootstrap-onyx-noteair

What it takes to get GlassineOS onto one device, the Onyx Boox Note Air (SDM636):
the boot loader changes, the partition layout, the recovery's device tree, and the
steps to install, repair and go back to stock. **Empty so far.**

## What will go here

- **Boot loader:** the changes to the device's UEFI boot loader (ABL), with the
  build and signing steps. A boot loader that doesn't start leaves the device
  reachable only over the Qualcomm emergency download mode, so the recipes come with
  the recovery steps.
- **Partition layout:** the A/B partition table and the tools that build and check it.
- **Recovery:** the device tree for the recovery
  ([android_device_onyx_noteair](https://github.com/GlassineOS/android_device_onyx_noteair)
  holds it today).
- **Emergency download recipes:** reading and writing partitions when nothing else
  boots.
- **Install and go back:** from stock to GlassineOS, and from GlassineOS back to stock.

Nothing vendor-owned goes here: no firmware, boot loader binaries, partition dumps or
decompiler output. Where a step needs a vendor file, it takes it from the user's own
device.

## Waiting for

The root file system model of GlassineOS. The install steps write that layout, so it
has to be decided and tried on a device first.

## License

GPL-2.0-or-later (`LICENSE`), except where a file says otherwise (boot loader patches
keep the license of the code they change).
