

- SceneKit
- SCNNode
-  light 

Instance Property

# light

The light attached to the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var light: SCNLight? { get set }
```

## Discussion

A node can have only one light attached to it. To combine lights so they can be controlled or animated together, create a node with no light and add other nodes to it.

## See Also

### Managing Node Content

var name: String?

A name associated with the node.

var camera: SCNCamera?

The camera attached to the node.

var geometry: SCNGeometry?

The geometry attached to the node.

var morpher: SCNMorpher?

The morpher object responsible for blending the node’s geometry.

var skinner: SCNSkinner?

The skinner object responsible for skeletal animations of node’s contents.

var categoryBitMask: Int

A mask that defines which categories the node belongs to.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

