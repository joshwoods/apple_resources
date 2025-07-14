

- ARKit
- AREnvironmentProbeAnchor
-  environmentTexture 

Instance Property

# environmentTexture

A cube-map texture that represents the view in all directions from the probe anchor’s position.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var environmentTexture: (any MTLTexture)? { get }
```

## Discussion

This texture is in the format MTLPixelFormat.bgra8Unorm_srgb.

