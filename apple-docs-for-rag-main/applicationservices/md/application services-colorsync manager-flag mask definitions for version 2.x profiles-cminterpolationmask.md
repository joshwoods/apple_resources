

- Application Services
- ColorSync Manager
- Flag Mask Definitions for Version 2.x Profiles
-  cmInterpolationMask 

Global Variable

# cmInterpolationMask

macOS 10.0+

``` source
var cmInterpolationMask: Int { get }
```

## Discussion

This mask provides access to bit 18 of the `flags` field, which specifies whether to use interpolation in color matching. The value 0 specifies interpolation. The value 1 specifies table lookup without interpolation. Specifying lookup only improves speed but can reduce accuracy. You might use lookup only for a monitor profile, for example, when high resolution is not crucial.

This feature is provided by the ColorSync Manager; it is not defined by the ICC profile specification.

