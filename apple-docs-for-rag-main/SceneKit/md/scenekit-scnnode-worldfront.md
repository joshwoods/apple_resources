

- SceneKit
- SCNNode
-  worldFront 

Instance Property

# worldFront

The “forward” (-Z) direction vector relative to the node, expressed in world space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var worldFront: SCNVector3 { get }
```

## Discussion

Reading this property is equivalent to reading the localFront class property and using the convertVector(_:to:) or convertVector(_:from:) method to convert that vector from the node’s local coordinate space to the scene’s world coordinate space.

## See Also

### Related Documentation

var simdWorldFront: simd_float3

The “forward” (-Z) direction vector relative to the node, expressed in world space.

### Calculating Node-Relative Transforms (SceneKit Types)

class var localRight: SCNVector3

The direction SceneKit treats as “right” in local space for all nodes.

class var localUp: SCNVector3

The direction SceneKit treats as “up” in local space for all nodes.

class var localFront: SCNVector3

The unit vector SceneKit treats as “forward” in local space for all nodes.

var worldRight: SCNVector3

The “right” (+X) direction vector relative to the node, expressed in world space.

var worldUp: SCNVector3

The “up” (+Y) direction vector relative to the node, expressed in world space.

