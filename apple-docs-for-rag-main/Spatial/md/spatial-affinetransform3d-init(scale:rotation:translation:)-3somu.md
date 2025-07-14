

- Spatial
- AffineTransform3D
-  init(scale:rotation:translation:) 

Initializer

# init(scale:rotation:translation:)

Creates an affine transform from the specified scale, rotate, and translate transforms.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    scale: Size3D = Size3D(width: 1.0, height: 1, depth: 1),
    rotation: Rotation3D = .zero,
    translation: Vector3D = .zero
)
```

## Parameters 

`scale`  

A size structure that specifies the scale.

`rotation`  

A rotation structure that specifies the rotation.

`translation`  

A vector that specifies the translation.

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

