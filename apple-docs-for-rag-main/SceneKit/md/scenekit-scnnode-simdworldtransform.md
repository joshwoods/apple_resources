

- SceneKit
- SCNNode
-  simdWorldTransform 

Instance Property

# simdWorldTransform

The world transform applied to the node.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdWorldTransform: simd_float4x4 { get set }
```

## Discussion

A world transform is the node’s coordinate space transform relative to the scene’s coordinate space. This transform is the concatenation of the node’s simdTransform property with that of its parent node, the parent’s parent, and so on up to the rootNode object of the scene.

## See Also

### Related Documentation

var worldTransform: SCNMatrix4

The world transform applied to the node.

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

### Managing Transforms in World Space

var simdWorldOrientation: simd_quatf

The node’s orientation relative to the scene’s world coordinate space.

var simdWorldPosition: simd_float3

The node’s position relative to the scene’s world coordinate space.

