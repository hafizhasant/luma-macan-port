# Luma Mobile port target: OnePlus 15R (macan)

- Device: OnePlus 15R
- Indian model: CPH2767
- Codename: macan
- SoC family: Qualcomm SM8850
- Reference OS: LineageOS 24
- Kernel base: 6.12 / Android 17 LineageOS stack
- Build goal: RAM-only Luma test image using fastboot boot
- Flashing: NOT allowed until RAM boot is proven

## Required repositories
- https://github.com/OnePlus-SM8850-Development/android_device_oneplus_macan-kernel
- https://github.com/OnePlus-SM8850-Development/android_device_oneplus_sm8850-common
- Matching LineageOS 24 kernel/common/modules/devicetree repositories

## Safety rules
- Never flash the generic Luma system.
- Never write vbmeta.
- Never touch persist, modemst1, modemst2, or fsg.
- First test must be: fastboot boot luma-macan-test.img
