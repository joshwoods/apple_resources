

- SceneKit
- SCNNode
-  simdLocalRight 

Type Property

# simdLocalRight

The direction SceneKit treats as “right” in local space for all nodes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class var simdLocalRight: simd_float3 { get }
```

## Discussion

No SceneKit features depend directly on this direction’s definition—it’s simply a natural consequence of recognizing “forward” and “up” directions for use with cameras, directional lighting, and relative orientation operations.

This vector is always `(1, 0, 0)` for all nodes, but you can use this class property when it’s convenient to refer to directions symbolically.

## See Also

### Related Documentation

class var localRight: SCNVector3

The direction SceneKit treats as “right” in local space for all nodes.

### Calculating Node-Relative Transforms

class var simdLocalUp: simd_float3

The direction SceneKit treats as “up” in local space for all nodes.

class var simdLocalFront: simd_float3

The unit vector SceneKit treats as “forward” in local space for all nodes.

var simdWorldRight: simd_float3

The “right” (+X) direction vector relative to the node, expressed in world space.

var simdWorldUp: simd_float3

The “up” (+Y) direction vector relative to the node, expressed in world space.

var simdWorldFront: simd_float3

The “forward” (-Z) direction vector relative to the node, expressed in world space.

