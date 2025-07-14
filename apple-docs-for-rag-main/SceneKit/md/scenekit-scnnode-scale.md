

- SceneKit
- SCNNode
-  scale 

Instance Property

# scale

The scale factor applied to the node. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var scale: SCNVector3 { get set }
```

## Discussion

Each component of the scale vector multiplies the corresponding dimension of the node’s geometry. The default scale is `1.0` in all three dimensions. For example, applying a scale of (2.0, 0.5, 2.0) to a node containing a cube geometry reduces its height and increases its width and depth. Scaling is applied relative to the node’s pivot property.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var simdScale: simd_float3

The scale factor applied to the node. Animatable.

### Managing the Node’s Transform (SceneKit Types)

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

var position: SCNVector3

The translation applied to the node. Animatable.

var rotation: SCNVector4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var eulerAngles: SCNVector3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var orientation: SCNQuaternion

The node’s orientation, expressed as a quaternion. Animatable.

var pivot: SCNMatrix4

The pivot point for the node’s position, rotation, and scale. Animatable.

