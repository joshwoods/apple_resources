

- Spatial
- Rotation3D
-  angle 

Instance Property

# angle

The angle of the rotation.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var angle: Angle2D { get set }
```

## See Also

### Inspecting a 3D rotation’s properties

var axis: RotationAxis3D

The axis of the rotation.

func eulerAngles(order: __SPEulerAngleOrder) -> EulerAngles

Returns a rotation’s Euler angles.

struct EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

var quaternion: simd_quatd

A quaternion that represents the rotation.

var vector: simd_double4

The underlying vector of the rotation.

