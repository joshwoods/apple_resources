

- Spatial
- Rotation3D
-  eulerAngles(order:) 

Instance Method

# eulerAngles(order:)

Returns a rotation’s Euler angles.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func eulerAngles(order: __SPEulerAngleOrder) -> EulerAngles
```

## Parameters 

`order`  

The Euler angle ordering.

## Return Value

A structure that represents Euler angles and ordering.

## See Also

### Inspecting a 3D rotation’s properties

var angle: Angle2D

The angle of the rotation.

var axis: RotationAxis3D

The axis of the rotation.

struct EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

var quaternion: simd_quatd

A quaternion that represents the rotation.

var vector: simd_double4

The underlying vector of the rotation.

