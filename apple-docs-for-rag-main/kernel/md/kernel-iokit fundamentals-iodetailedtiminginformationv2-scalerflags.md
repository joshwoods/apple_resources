

- Kernel
- IOKit Fundamentals
- IODetailedTimingInformationV2
-  scalerFlags 

Instance Property

# scalerFlags

If the mode is scaled, kIOScaleStretchToFit may be set to allow stretching. kIOScaleRotateFlags is mask which may have the value given by kIOScaleRotate90, kIOScaleRotate180, kIOScaleRotate270 to display a rotated framebuffer.

macOS 10.1+

``` source
UInt32 scalerFlags;
```

