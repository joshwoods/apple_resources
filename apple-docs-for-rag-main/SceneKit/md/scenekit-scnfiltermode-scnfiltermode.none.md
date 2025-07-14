

- SceneKit
- SCNFilterMode
-  SCNFilterMode.none 

Case

# SCNFilterMode.none

No texture filtering is applied.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
case none
```

## Discussion

Only valid for the mipFilter property, specifying that SceneKit should not use mip mapping.

## See Also

### Constants

case nearest

Texture filtering returns the color from only one texel, whose location is nearest to the coordinates being sampled.

case linear

Texture filtering sample texels from the neighborhood of the coordinates being sampled and linearly interpolates their colors.

