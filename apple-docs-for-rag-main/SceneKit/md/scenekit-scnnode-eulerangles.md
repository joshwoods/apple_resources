

- SceneKit
- SCNNode
-  eulerAngles 

Instance Property

# eulerAngles

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var eulerAngles: SCNVector3 { get set }
```

## Discussion

The order of components in this vector matches the axes of rotation:

- Pitch (the `x` component) is the rotation about the node’s x-axis.

- Yaw (the `y` component) is the rotation about the node’s y-axis.

- Roll (the `z` component) is the rotation about the node’s z-axis.

SceneKit applies these rotations relative to the node’s pivot property in the reverse order of the components: first roll, then yaw, then pitch. The rotation, eulerAngles, and orientation properties all affect the rotational aspect of the node’s transform property. Any change to one of these properties is reflected in the others.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var simdEulerAngles: simd_float3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

### Managing the Node’s Transform (SceneKit Types)

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

var position: SCNVector3

The translation applied to the node. Animatable.

var rotation: SCNVector4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var orientation: SCNQuaternion

The node’s orientation, expressed as a quaternion. Animatable.

var scale: SCNVector3

The scale factor applied to the node. Animatable.

var pivot: SCNMatrix4

The pivot point for the node’s position, rotation, and scale. Animatable.

