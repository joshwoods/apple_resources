

- SceneKit
- SCNNode
-  worldPosition 

Instance Property

# worldPosition

The node’s position relative to the scene’s world coordinate space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var worldPosition: SCNVector3 { get set }
```

## Discussion

This vector isolates the translational aspect of the node’s worldTransform matrix, which in turn is the conversion of the node’s transform from local space to the scene’s world coordinate space. That is, it expresses the x, y, and z offsets of the node’s position from that of the scene’s rootNode, and is equivalent to reading the node’s position vector and converting it to world space with the convertPosition(_:from:) or convertPosition(_:to:) method.

## See Also

### Related Documentation

var simdWorldPosition: simd_float3

The node’s position relative to the scene’s world coordinate space.

### Managing Transforms in World Space (SceneKit Types)

var worldTransform: SCNMatrix4

The world transform applied to the node.

func setWorldTransform(SCNMatrix4)

Sets the world transform applied to the node.

var worldOrientation: SCNQuaternion

The node’s orientation relative to the scene’s world coordinate space.

