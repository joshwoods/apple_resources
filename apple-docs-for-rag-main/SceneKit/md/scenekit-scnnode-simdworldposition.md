

- SceneKit
- SCNNode
-  simdWorldPosition 

Instance Property

# simdWorldPosition

The node’s position relative to the scene’s world coordinate space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdWorldPosition: simd_float3 { get set }
```

## Discussion

This vector isolates the translational aspect of the node’s simdWorldTransform matrix, which in turn is the conversion of the node’s simdTransform from local space to the scene’s world coordinate space. That is, it expresses the x, y, and z offsets of the node’s position from that of the scene’s rootNode, and is equivalent to reading the node’s simdPosition vector and converting it to world space with the simdConvertPosition(_:from:) or simdConvertPosition(_:to:) method.

## See Also

### Related Documentation

var worldPosition: SCNVector3

The node’s position relative to the scene’s world coordinate space.

### Managing Transforms in World Space

var simdWorldTransform: simd_float4x4

The world transform applied to the node.

var simdWorldOrientation: simd_quatf

The node’s orientation relative to the scene’s world coordinate space.

