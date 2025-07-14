

- SceneKit
- SCNFilterMode
-  SCNFilterMode.nearest 

Case

# SCNFilterMode.nearest

Texture filtering returns the color from only one texel, whose location is nearest to the coordinates being sampled.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
case nearest
```

## See Also

### Constants

case none

No texture filtering is applied.

case linear

Texture filtering sample texels from the neighborhood of the coordinates being sampled and linearly interpolates their colors.

