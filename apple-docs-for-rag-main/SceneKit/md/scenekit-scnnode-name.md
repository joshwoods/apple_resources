

- SceneKit
- SCNNode
-  name 

Instance Property

# name

A name associated with the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var name: String? { get set }
```

## Discussion

You can provide a descriptive name for a node to make managing your scene graph easier. Nodes loaded from a scene file may have names assigned by an artist using a 3D authoring tool. Use the childNode(withName:recursively:) or childNodes(passingTest:) method to retrieve a node from a scene graph by its name, or the SCNSceneSource class to examine nodes in a scene file without loading its scene graph.

The names of nodes and their attached objects are saved when you export a scene to a file using its write(to:options:delegate:progressHandler:) method, and appear in the Xcode scene editor. The SceneKit statistics view (see showsStatistics) also shows the names of nodes with attached cameras.

## See Also

### Related Documentation

func childNodes(passingTest: (SCNNode, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [SCNNode]

Returns all nodes in the node’s child node subtree that satisfy the test applied by a block.

func childNode(withName: String, recursively: Bool) -> SCNNode?

Returns the first node in the node’s child node subtree with the specified name.

### Managing Node Content

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

var categoryBitMask: Int

A mask that defines which categories the node belongs to.

protocol SCNBoundingVolume

Methods common to the SCNNode and SCNGeometry classes for measuring location and size.

