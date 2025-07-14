

- SceneKit
- SCNNode
-  geometry 

Instance Property

# geometry

The geometry attached to the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var geometry: SCNGeometry? { get set }
```

## Discussion

A node can have only one geometry attached to it. To combine geometries so they can be controlled or animated together, create a node with no geometry and add other nodes to it.

Animating the node’s geometric properties can move, rotate, stretch and scale its geometry. For more advanced animations of a node’s geometry, use its morpher and skinner objects.

## See Also

### Managing Node Content

var name: String?

A name associated with the node.

var light: SCNLight?

The light attached to the node.

var camera: SCNCamera?

The camera attached to the node.

var morpher: SCNMorpher?

The morpher object responsible for blending the node’s geometry.

var skinner: SCNSkinner?

The skinner object responsible for skeletal animations of node’s contents.

var categoryBitMask: Int

A mask that defines which categories the node belongs to.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

