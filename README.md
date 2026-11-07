# NidhiKernel AnyKernel3

AnyKernel3 installer for [NidhiKernel](https://github.com/kaixenberg/kernel_xiaomi_sm8250) on alioth
(POCO F3 / Mi 11X / Redmi K40). Forked from TIMISONG-dev's
[MagicTime-alioth](https://github.com/TIMISONG-dev/MagicTime-alioth).

The zip flashes `Image` and `dtbo.img` to the active slot's `boot` and
`dtbo`. It leaves `vendor_boot` alone: the base dtb there comes from the
ROM, and all kernel-side devicetree changes for alioth live in the dtbo
overlay.

Credits: osm0sis for AnyKernel3, TIMISONG-dev for MagicTime.
