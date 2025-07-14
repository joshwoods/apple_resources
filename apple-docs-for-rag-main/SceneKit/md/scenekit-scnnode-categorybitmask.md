

- SceneKit
- SCNNode
-  categoryBitMask 

Instance Property

# categoryBitMask

A mask that defines which categories the node belongs to.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var categoryBitMask: Int { get set }
```

## Discussion

You can assign each node in a scene to one or more categories, where each category corresponds to a bit in the bit mask. You define the mask values used in your app. When SceneKit renders a scene, it compares each node’s categoryBitMask property with the category bit masks of every other object that participates in the rendering process—lights, cameras, and techniques—using a bitwise AND operation. If the result is a nonzero value, SceneKit includes the node when rendering. The default category bit mask is `1`.

Use a node’s category bit mask together with:

- An SCNLight object’s categoryBitMask property to exclude the node from that light’s illumination

- An SCNCamera object’s categoryBitMask property to make the node invisible to that camera

- The category bit masks in an SCNTechnique object’s definition dictionary to include or exclude the node from phases of a multipass rendering technique

Note

This property doesn’t affect SceneKit’s physics simulation. To include or exclude a node from physics interactions, use the categoryBitMask property of the node’s physicsBody and physicsField objects.

## See Also

### Managing Node Content

var name: String?

A name associated with the node.

var light: SCNLight?

The light attached to the node.

var camera: SCNCamera?

The camera attached to the node.

var geometry: SCNGeometry?

The geometry attached to the node.

var morpher: SCNMorpher?

The morpher object responsible for blending the node’s geometry.

var skinner: SCNSkinner?

The skinner object responsible for skeletal animations of node’s contents.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

