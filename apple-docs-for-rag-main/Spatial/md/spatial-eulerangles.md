

- Spatial
-  EulerAngles 

Structure

# EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EulerAngles
```

## Topics

### Initializers

init()

Creates a new Euler angles structure.

init(angles: simd_float3, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified single-precision angles and order.

init(angles: simd_double3, order: __SPEulerAngleOrder)

Creates a new Euler angles structure from the specified double-precision angles and order.

init(x: Angle2D, y: Angle2D, z: Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

init(Angle2D, Angle2D, Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

Deprecated

### Instance properties

var angles: simd_double3

A three-element vector that specifies the Euler angles.

var order: __SPEulerAngleOrder

The Euler angle order.

var angles: simd_double3

A three-element vector that specifies the Euler angles.

var order: __SPEulerAngleOrder

The Euler angle order.

### Supporting types

typealias Order

A type that specifies the order of the angles.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating a 3D rotation structure

init()

Creates a rotation.

init()

Creates a rotation structure.

init(eulerAngles: EulerAngles)

Creates a rotation structure with the specified Euler angles.

init(eulerAngles: EulerAngles)

Creates a rotation structure with the specified Euler angles.

init(quaternion: simd_quatd)

Creates a rotation axis from the specified double-precision quaternion.

init(simd_quatd)

Creates a rotation from the specified double-precision quaternion.

init(simd_quatf)

Creates a rotation axis from the specified single-precision quaternion.

init(angle: Angle2D, axis: RotationAxis3D)

Creates a rotation structure with the specified axis and the specified angle from Spatial structures.

init(position: Point3D, target: Point3D, up: Vector3D)

Creates a rotation structure that represents the look-at direction from a position to a target.

init(forward: Vector3D)

Creates a rotation with the specified forward vector.

init(forward: Vector3D, up: Vector3D)

Creates a rotation with the specified forward and up vectors.

init(forward: Vector3D, up: Vector3D)

Creates a rotation with the specified forward and up vectors.

