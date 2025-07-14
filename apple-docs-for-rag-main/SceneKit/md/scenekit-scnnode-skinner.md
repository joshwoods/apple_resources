

- SceneKit
- SCNNode
-  skinner 

Instance Property

# skinner

The skinner object responsible for skeletal animations of node’s contents.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var skinner: SCNSkinner? { get set }
```

## Discussion

A skinner object maintains an hierarchy of control nodes that can deform the node’s geometry using skeletal animations created in an external 3D authoring tool. For details, see SCNSkinner.

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

var categoryBitMask: Int

A mask that defines which categories the node belongs to.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

