

- SceneKit
- SCNNode
-  simdPosition 

Instance Property

# simdPosition

The translation applied to the node. Animatable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var simdPosition: simd_float3 { get set }
```

## Discussion

The node’s position locates it within the coordinate system of its parent, as modified by the node’s simdPivot property. The default position is the zero vector, indicating that the node is placed at the origin of the parent node’s coordinate system.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var position: SCNVector3

The translation applied to the node. Animatable.

### Managing the Node’s Transform

var simdTransform: simd_float4x4

The transform applied to the node relative to its parent. Animatable.

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

