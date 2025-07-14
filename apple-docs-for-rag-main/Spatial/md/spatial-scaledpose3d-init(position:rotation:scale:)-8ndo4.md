

- Spatial
- ScaledPose3D
-  init(position:rotation:scale:) 

Initializer

# init(position:rotation:scale:)

Creates a scaled pose with the specified single-precision position vector and quaternion.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
init(
    position: simd_float3 = .zero,
    rotation: simd_quatf,
    scale: Float = 1
)
```

## See Also

### Creating a 3D scaled-pose structure

init()

Creates a scaled pose structure.

init?(simd_float4x4)

Creates a scaled pose from the specified 4 x 4 single-precision matrix.

init?(simd_double4x4)

Creates a scaled pose from the specified 4 x 4 double-precision matrix.

init(forward: Vector3D, scale: Double, up: Vector3D)

Creates a scaled pose with the specified forward and up vectors.

init(position: simd_double3, rotation: simd_quatd, scale: Double)

Creates a scaled pose with the specified double-precision position vector and quaternion.

init(position: Point3D, target: Point3D, scale: Double, up: Vector3D)

Returns a scaled pose at the specified position with the rotation toward the target.

init(position: Point3D, rotation: Rotation3D, scale: Double)

Creates a pose with the specified Spatial position, rotation, and scale structures.

init(position: Point3D, rotation: Rotation3D, scale: Double)

Creates a scaled pose with the specified double-precision position vector and quaternion.

init?(transform: AffineTransform3D)

Returns a scaled pose with a position, rotation, and scale defined by an affine transform.

init?(transform: ProjectiveTransform3D)

Returns a scaled pose with a position, rotation, and scale defined by a projective transform.

