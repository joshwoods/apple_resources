

- SceneKit
- SCNNode
-  morpher 

Instance Property

# morpher

The morpher object responsible for blending the node’s geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var morpher: SCNMorpher? { get set }
```

## Discussion

You use a morpher object to interpolate between multiple geometries. For details, see SCNMorpher.

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

var skinner: SCNSkinner?

The skinner object responsible for skeletal animations of node’s contents.

var categoryBitMask: Int

A mask that defines which categories the node belongs to.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

