

- SceneKit
- SCNNode
-  orientation 

Instance Property

# orientation

The node’s orientation, expressed as a quaternion. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var orientation: SCNQuaternion { get set }
```

## Discussion

The rotation, eulerAngles, and orientation properties all affect the rotational aspect of the node’s transform property. Any change to one of these properties is reflected in the others.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var simdOrientation: simd_quatf

The node’s orientation, expressed as a quaternion. Animatable.

### Managing the Node’s Transform (SceneKit Types)

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

var position: SCNVector3

The translation applied to the node. Animatable.

var rotation: SCNVector4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var eulerAngles: SCNVector3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var scale: SCNVector3

The scale factor applied to the node. Animatable.

var pivot: SCNMatrix4

The pivot point for the node’s position, rotation, and scale. Animatable.

