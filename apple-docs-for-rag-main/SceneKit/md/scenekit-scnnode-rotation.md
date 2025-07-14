

- SceneKit
- SCNNode
-  rotation 

Instance Property

# rotation

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rotation: SCNVector4 { get set }
```

## Discussion

The four-component rotation vector specifies the direction of the rotation axis in the first three components and the angle of rotation (in radians) in the fourth. The default rotation is the zero vector, specifying no rotation. Rotation is applied relative to the node’s pivot property.

The rotation, eulerAngles, and orientation properties all affect the rotational aspect of the node’s transform property. Any change to one of these properties is reflected in the others.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var simdRotation: simd_float4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

### Managing the Node’s Transform (SceneKit Types)

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

var position: SCNVector3

The translation applied to the node. Animatable.

var eulerAngles: SCNVector3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var orientation: SCNQuaternion

The node’s orientation, expressed as a quaternion. Animatable.

var scale: SCNVector3

The scale factor applied to the node. Animatable.

var pivot: SCNMatrix4

The pivot point for the node’s position, rotation, and scale. Animatable.

