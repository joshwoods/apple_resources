

- ARKit
- EnvironmentProbeAnchor
-  environmentTexture 

Instance Property

# environmentTexture

The environment texture of an anchor.

visionOS 2.0+

``` source
var environmentTexture: (any MTLTexture)? { get }
```

## Discussion

Textures may be `nil` if the person isn’t in a well-lit environment.

## See Also

### Getting anchor information

var cameraScaleReference: Float

The camera scale reference of this anchor.

var originFromAnchorTransform: simd_float4x4

The transform from the environment probe anchor to the origin coordinate system.

