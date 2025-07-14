

- SceneKit
- SCNNode
-  simdEulerAngles 

Instance Property

# simdEulerAngles

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdEulerAngles: simd_float3 { get set }
```

## Discussion

The order of components in this vector matches the axes of rotation:

- Pitch (the `x` component) is the rotation about the node’s x-axis.

- Yaw (the `y` component) is the rotation about the node’s y-axis.

- Roll (the `z` component) is the rotation about the node’s z-axis.

SceneKit applies these rotations relative to the node’s simdPivot property in the reverse order of the components: first roll, then yaw, then pitch. The simdRotation, simdEulerAngles, and simdOrientation properties all affect the rotational aspect of the node’s simdTransform property. Any change to one of these properties is reflected in the others.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var eulerAngles: SCNVector3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

### Managing the Node’s Transform

var simdTransform: simd_float4x4

The transform applied to the node relative to its parent. Animatable.

var simdPosition: simd_float3

The translation applied to the node. Animatable.

var simdRotation: simd_float4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var simdOrientation: simd_quatf

The node’s orientation, expressed as a quaternion. Animatable.

var simdScale: simd_float3

The scale factor applied to the node. Animatable.

var simdPivot: simd_float4x4

The pivot point for the node’s position, rotation, and scale. Animatable.

