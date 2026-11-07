# NidhiKernel AnyKernel3

AnyKernel3 installer for [NidhiKernel](https://github.com/kaixenberg/kernel_xiaomi_sm8250) on alioth
(POCO F3 / Mi 11X / Redmi K40). Forked from TIMISONG-dev's
[MagicTime-alioth](https://github.com/TIMISONG-dev/MagicTime-alioth).

The zip flashes `Image` and `dtbo.img` to the active slot's `boot` and
`dtbo`. On alioth it leaves `vendor_boot` alone: the base dtb there comes
from the ROM, and all kernel-side devicetree changes live in the dtbo
overlay.

A zip that also contains a `dtb` file gets it written into `vendor_boot`
by AnyKernel3's automatic hdr v3 handling. The kernel's build workflow
adds one only for pipa builds. It also sets the `device.name` lines for
the device a zip was built for; this repo's defaults are alioth's.

Credits: osm0sis for AnyKernel3, TIMISONG-dev for MagicTime.
