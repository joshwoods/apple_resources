

- SceneKit
- SCNNode
-  transform 

Instance Property

# transform

The transform applied to the node relative to its parent. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
var transform: SCNMatrix4 { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
var transform: SCNMatrix4 { get set }
```

## Discussion

The transformation is the combination of the node’s rotation, position, and scale properties. The default transformation is SCNMatrix4Identity.

When you set the value of this property, the node’s rotation, orientation, eulerAngles, position, and scale properties automatically change to match the new transform, and vice versa. SceneKit can perform this conversion only if the transform you provide is a combination of rotation, translation, and scale operations. If you set the value of this property to a skew transformation or to a nonaffine transformation, the values of these properties become undefined. Setting a new value for any of these properties causes SceneKit to compute a new transformation, discarding any skew or nonaffine operations in the original transformation.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var simdTransform: simd_float4x4

The transform applied to the node relative to its parent. Animatable.

### Managing the Node’s Transform (SceneKit Types)

var position: SCNVector3

The translation applied to the node. Animatable.

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

