

- SceneKit
- SCNNode
-  simdWorldOrientation 

Instance Property

# simdWorldOrientation

The node’s orientation relative to the scene’s world coordinate space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdWorldOrientation: simd_quatf { get set }
```

## Discussion

This quaternion isolates the rotational aspect of the node’s simdWorldTransform matrix, which in turn is the conversion of the node’s simdTransform from local space to the scene’s world coordinate space. That is, it expresses the difference in axis and angle of rotation between the node and the scene’s rootNode.

## See Also

### Related Documentation

var worldOrientation: SCNQuaternion

The node’s orientation relative to the scene’s world coordinate space.

### Managing Transforms in World Space

var simdWorldTransform: simd_float4x4

The world transform applied to the node.

var simdWorldPosition: simd_float3

The node’s position relative to the scene’s world coordinate space.

