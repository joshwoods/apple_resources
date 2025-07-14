

- SceneKit
- SCNNode
-  simdOrientation 

Instance Property

# simdOrientation

The node’s orientation, expressed as a quaternion. Animatable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdOrientation: simd_quatf { get set }
```

## Discussion

The simdRotation, simdEulerAngles, and simdOrientation properties all affect the rotational aspect of the node’s simdTransform property. Any change to one of these properties is reflected in the others.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var orientation: SCNQuaternion

The node’s orientation, expressed as a quaternion. Animatable.

### Managing the Node’s Transform

var simdTransform: simd_float4x4

The transform applied to the node relative to its parent. Animatable.

var simdPosition: simd_float3

The translation applied to the node. Animatable.

var simdRotation: simd_float4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var simdEulerAngles: simd_float3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var simdScale: simd_float3

The scale factor applied to the node. Animatable.

var simdPivot: simd_float4x4

The pivot point for the node’s position, rotation, and scale. Animatable.

