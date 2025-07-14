

- SceneKit
- SCNNode
-  setWorldTransform(\_:) 

Instance Method

# setWorldTransform(\_:)

Sets the world transform applied to the node.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func setWorldTransform(_ worldTransform: SCNMatrix4)
```

**macOS**

``` source
func setWorldTransform(_ worldTransform: SCNMatrix4)
```

## Parameters 

`worldTransform`  

The new transform matrix, relative to the scene coordinate space, to apply to the node.

## Discussion

A world transform is the node’s coordinate space transform relative to the scene’s coordinate space. This transform is the concatenation of the node’s transform property with that of its parent node, the parent’s parent, and so on up to the rootNode object of the scene.

## See Also

### Related Documentation

var simdWorldTransform: simd_float4x4

The world transform applied to the node.

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

### Managing Transforms in World Space (SceneKit Types)

var worldTransform: SCNMatrix4

The world transform applied to the node.

var worldOrientation: SCNQuaternion

The node’s orientation relative to the scene’s world coordinate space.

var worldPosition: SCNVector3

The node’s position relative to the scene’s world coordinate space.

