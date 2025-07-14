

- Spatial
- AffineTransform3D
-  init(truncating:) 

Initializer

# init(truncating:)

Returns a new affine transform structure from the specified 4 x 4 matrix truncated to a 4 x 3 matrix.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(truncating matrix: simd_double4x4)
```

## See Also

### Creating a 3D affine transform structure

init()

Creates an affine transform.

init()

Returns a new identity affine transform.

init(simd_float4x3)

Creates an affine transform from the specified single-precision matrix.

init(simd_double4x3)

Creates an affine transform from the specified 4 x 3 double-precision matrix.

init(Transform)

Creates an affine transform from the specified transform.

init(matrix: simd_double4x3)

Creates an affine transform from the specified double-precision matrix.

init(pose: Pose3D)

Creates an affine transform from the specified pose structure.

init(rotation: Rotation3D)

Creates an affine transform from the specified rotate transform.

init(scale: Size3D)

Creates an affine transform from the specified scale transform.

init(scale: Size3D, rotation: Rotation3D, translation: Vector3D)

Creates an affine transform from the specified scale, rotate, and translate transforms.

init(scaledPose: ScaledPose3D)

Creates an affine transform from the specified scale pose structure.

init(shear: AxisWithFactors)

Creates an affine transform from the specified shear transform.

init(translation: Vector3D)

Creates an affine transform from the specified translate transform.

init(truncating: ProjectiveTransform3D)

Returns a new affine transform structure from the specified projective transform.

init(truncating: simd_float4x4)

Returns a new affine transform structure from the specified single-precision 4 x 4 matrix truncated to a 4 x 3 matrix.

