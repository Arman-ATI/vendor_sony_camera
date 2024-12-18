# vendor_sony_camera

Prebuilt stock Sony Camera for msm8998 devices (maple and maple_dsds) to include in custom ROM builds.

### How to use?

1. Clone this repo to `vendor/sony/camera`

2. Inherit it from `device.mk` in device tree:

```
# Camera
$(call inherit-product-if-exists, vendor/sony/camera/sony-camera.mk)
```

3. Ensure that the PRODUCT_BRAND is sony and that it is not overriden by any of the safetynet hacks.
