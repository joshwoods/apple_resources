

- SceneKit
- SCNNode
-  position 

Instance Property

# position

The translation applied to the node. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var position: SCNVector3 { get set }
```

## Discussion

The node’s position locates it within the coordinate system of its parent, as modified by the node’s pivot property. The default position is the zero vector, indicating that the node is placed at the origin of the parent node’s coordinate system.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var simdPosition: simd_float3

The translation applied to the node. Animatable.

### Managing the Node’s Transform (SceneKit Types)

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

var rotation: SCNVector4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var eulerAngles: SCNVector3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var orientation: SCNQuaternion

The node’s orientation, expressed as a quaternion. Animatable.

var scale: SCNVector3

The scale factor applied to the node. Animatable.

var pivot: SCNMatrix4

The pivot point for the node’s position, rotation, and scale. Animatable.

