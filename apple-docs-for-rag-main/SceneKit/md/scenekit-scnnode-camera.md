

- SceneKit
- SCNNode
-  camera 

Instance Property

# camera

The camera attached to the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var camera: SCNCamera? { get set }
```

## Discussion

To use a camera for displaying a scene, set the the pointOfView property of the view (or layer or renderer) displaying the scene to the node containing the camera. A camera looks in the direction of the node’s negative z-axis, so you aim the camera by changing the position and orientation of the node containing it. You control geometric and optical parameters of the camera—projection, field of view, and depth of field—using the attached SCNCamera object.

## See Also

### Managing Node Content

var name: String?

A name associated with the node.

var light: SCNLight?

The light attached to the node.

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

