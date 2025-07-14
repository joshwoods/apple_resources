

- Spatial
- Rotation3D
-  init(\_:) 

Initializer

# init(\_:)

Creates a rotation from the specified double-precision quaternion.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(_ quaternion: simd_quatd)
```

## Parameters 

`quaternion`  

A double-precision quaternion that specifies the rotation.

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

struct EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

init(quaternion: simd_quatd)

Creates a rotation axis from the specified double-precision quaternion.

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

