

- SceneKit
- SCNNode
-  localUp 

Type Property

# localUp

The direction SceneKit treats as “up” in local space for all nodes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class var localUp: SCNVector3 { get }
```

## Discussion

The “up” direction of a node affects cameras attached to a node, as well as relative orientation and movement effects such as look(at:), SCNLookAtConstraint, and SCNBillboardConstraint.

This vector is always `(0, 1, 0)` for all nodes, but you can use this class property when it’s convenient to refer to directions symbolically.

## See Also

### Related Documentation

class var simdLocalUp: simd_float3

The direction SceneKit treats as “up” in local space for all nodes.

### Calculating Node-Relative Transforms (SceneKit Types)

class var localRight: SCNVector3

The direction SceneKit treats as “right” in local space for all nodes.

class var localFront: SCNVector3

The unit vector SceneKit treats as “forward” in local space for all nodes.

var worldRight: SCNVector3

The “right” (+X) direction vector relative to the node, expressed in world space.

var worldUp: SCNVector3

The “up” (+Y) direction vector relative to the node, expressed in world space.

var worldFront: SCNVector3

The “forward” (-Z) direction vector relative to the node, expressed in world space.

