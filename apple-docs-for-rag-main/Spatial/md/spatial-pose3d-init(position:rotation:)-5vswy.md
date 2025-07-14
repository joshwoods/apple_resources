

- Spatial
- Pose3D
-  init(position:rotation:) 

Initializer

# init(position:rotation:)

Creates a pose with the specified single-precision position vector and quaternion.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    position: Point3D = .zero,
    rotation: Rotation3D
)
```

## Parameters 

`position`  

A vector that specifies the position of the pose.

`rotation`  

A quaternion structure that specifies the rotation of the pose.

## See Also

### Creating a 3D pose structure

init()

Creates a pose structure.

init?(simd_float4x4)

Creates a pose from the specified 4 x 4 single-precision matrix.

init?(simd_double4x4)

Creates a pose from the specified 4 x 4 double-precision matrix.

init(forward: Vector3D, up: Vector3D)

Creates a pose with the specified forward and up vectors.

init(position: simd_float3, rotation: simd_quatf)

Creates a pose with the specified single-precision position vector and quaternion.

init(position: Point3D, rotation: Rotation3D)

Creates a pose with the specified Spatial position and rotation structures.

init(position: simd_double3, rotation: simd_quatd)

Creates a pose with the specified double-precision position vector and quaternion.

init(position: Point3D, target: Point3D, up: Vector3D)

Returns a pose at the specified position with the rotation towards the target.

init?(transform: AffineTransform3D)

Returns a pose with a position and rotation defined by an affine transform.

init?(transform: ProjectiveTransform3D)

Returns a pose with a position and rotation defined by a projective transform.

