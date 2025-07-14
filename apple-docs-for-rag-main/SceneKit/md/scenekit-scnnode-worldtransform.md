

- SceneKit
- SCNNode
-  worldTransform 

Instance Property

# worldTransform

The world transform applied to the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
var worldTransform: SCNMatrix4 { get }
```

**macOS**

``` source
var worldTransform: SCNMatrix4 { get }
```

## Discussion

A world transform is the node’s coordinate space transform relative to the scene’s coordinate space. This transform is the concatenation of the node’s transform property with that of its parent node, the parent’s parent, and so on up to the rootNode object of the scene.

Note

In macOS 10.13, iOS 11, tvOS 11, or watchOS 4 (and later), you can set this value with the setWorldTransform(_:) method.

## See Also

### Related Documentation

var simdWorldTransform: simd_float4x4

The world transform applied to the node.

var parent: SCNNode?

The node’s parent in the scene graph hierarchy.

### Managing Transforms in World Space (SceneKit Types)

func setWorldTransform(SCNMatrix4)

Sets the world transform applied to the node.

var worldOrientation: SCNQuaternion

The node’s orientation relative to the scene’s world coordinate space.

var worldPosition: SCNVector3

The node’s position relative to the scene’s world coordinate space.

