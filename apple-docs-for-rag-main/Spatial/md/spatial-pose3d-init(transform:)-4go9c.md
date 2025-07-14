

- Spatial
- Pose3D
-  init(transform:) 

Initializer

# init(transform:)

Returns a pose with a position and rotation defined by a projective transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init?(transform: ProjectiveTransform3D)
```

## Parameters 

`transform`  

The source transform. The function only considers the transform’s rotation and translation components.

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

init(position: Point3D, rotation: Rotation3D)

Creates a pose with the specified single-precision position vector and quaternion.

init(position: simd_double3, rotation: simd_quatd)

Creates a pose with the specified double-precision position vector and quaternion.

init(position: Point3D, target: Point3D, up: Vector3D)

Returns a pose at the specified position with the rotation towards the target.

init?(transform: AffineTransform3D)

Returns a pose with a position and rotation defined by an affine transform.

