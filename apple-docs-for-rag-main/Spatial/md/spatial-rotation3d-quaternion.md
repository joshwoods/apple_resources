

- Spatial
- Rotation3D
-  quaternion 

Instance Property

# quaternion

A quaternion that represents the rotation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var quaternion: simd_quatd { get set }
```

## See Also

### Inspecting a 3D rotation’s properties

var angle: Angle2D

The angle of the rotation.

var axis: RotationAxis3D

The axis of the rotation.

func eulerAngles(order: __SPEulerAngleOrder) -> EulerAngles

Returns a rotation’s Euler angles.

struct EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

var vector: simd_double4

The underlying vector of the rotation.

