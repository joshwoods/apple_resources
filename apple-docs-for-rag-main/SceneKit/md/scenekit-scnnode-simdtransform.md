

- SceneKit
- SCNNode
-  simdTransform 

Instance Property

# simdTransform

The transform applied to the node relative to its parent. Animatable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdTransform: simd_float4x4 { get set }
```

## Discussion

The transform is the combination of the node’s simdRotation, simdPosition, and simdScale properties. The default transform is the identity matrix.

When you set the value of this property, the node’s simdRotation, simdOrientation, simdEulerAngles, simdPosition, and simdScale properties automatically change to match the new transform, and vice versa. SceneKit can perform this conversion only if the transform you provide is a combination of rotation, translation, and scale operations. If you set the value of this property to a skew transform or to a nonaffine transform, the values of these properties become undefined. Setting a new value for any of these properties causes SceneKit to compute a new transform, discarding any skew or nonaffine operations in the original transform.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var transform: SCNMatrix4

The transform applied to the node relative to its parent. Animatable.

### Managing the Node’s Transform

var simdPosition: simd_float3

The translation applied to the node. Animatable.

var simdRotation: simd_float4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var simdEulerAngles: simd_float3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var simdOrientation: simd_quatf

The node’s orientation, expressed as a quaternion. Animatable.

var simdScale: simd_float3

The scale factor applied to the node. Animatable.

var simdPivot: simd_float4x4

The pivot point for the node’s position, rotation, and scale. Animatable.

