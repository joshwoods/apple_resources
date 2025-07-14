

- SceneKit
- SCNNode
-  simdLocalUp 

Type Property

# simdLocalUp

The direction SceneKit treats as “up” in local space for all nodes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class var simdLocalUp: simd_float3 { get }
```

## Discussion

The “up” direction of a node affects cameras attached to a node, as well as relative orientation and movement effects such as simdLook(at:), SCNLookAtConstraint, and SCNBillboardConstraint.

This vector is always `(0, 1, 0)` for all nodes, but you can use this class property when it’s convenient to refer to directions symbolically.

## See Also

### Related Documentation

class var localUp: SCNVector3

The direction SceneKit treats as “up” in local space for all nodes.

### Calculating Node-Relative Transforms

class var simdLocalRight: simd_float3

The direction SceneKit treats as “right” in local space for all nodes.

class var simdLocalFront: simd_float3

The unit vector SceneKit treats as “forward” in local space for all nodes.

var simdWorldRight: simd_float3

The “right” (+X) direction vector relative to the node, expressed in world space.

var simdWorldUp: simd_float3

The “up” (+Y) direction vector relative to the node, expressed in world space.

var simdWorldFront: simd_float3

The “forward” (-Z) direction vector relative to the node, expressed in world space.

