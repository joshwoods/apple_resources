

- Spatial
- AffineTransform3D
-  init(rotation:) 

Initializer

# init(rotation:)

Creates an affine transform from the specified rotate transform.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(rotation: Rotation3D)
```

## Parameters 

`rotation`  

A rotation structure that specifies the rotation.

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

init(truncating: simd_double4x4)

Returns a new affine transform structure from the specified 4 x 4 matrix truncated to a 4 x 3 matrix.

