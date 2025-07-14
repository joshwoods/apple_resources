

- SceneKit
- SCNNode
-  simdScale 

Instance Property

# simdScale

The scale factor applied to the node. Animatable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdScale: simd_float3 { get set }
```

## Discussion

Each component of the scale vector multiplies the corresponding dimension of the node’s geometry. The default scale is `1.0` in all three dimensions. For example, applying a scale of (2.0, 0.5, 2.0) to a node containing a cube geometry reduces its height and increases its width and depth. Scaling is applied relative to the node’s simdPivot property.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var scale: SCNVector3

The scale factor applied to the node. Animatable.

### Managing the Node’s Transform

var simdTransform: simd_float4x4

The transform applied to the node relative to its parent. Animatable.

var simdPosition: simd_float3

The translation applied to the node. Animatable.

var simdRotation: simd_float4

The node’s orientation, expressed as a rotation angle about an axis. Animatable.

var simdEulerAngles: simd_float3

The node’s orientation, expressed as pitch, yaw, and roll angles in radians. Animatable.

var simdOrientation: simd_quatf

The node’s orientation, expressed as a quaternion. Animatable.

var simdPivot: simd_float4x4

The pivot point for the node’s position, rotation, and scale. Animatable.

