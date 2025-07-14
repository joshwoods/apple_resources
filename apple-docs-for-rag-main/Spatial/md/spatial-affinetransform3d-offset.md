

- Spatial
- AffineTransform3D
-  offset 

Instance Property

# offset

The affine transform’s translation.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var offset: Vector3D { get set }
```

## See Also

### Deprecated symbols

init?(simd_float4x4)

Creates an affine transform from the specified 4 x 4 single-precision matrix.

Deprecated

init?(simd_double4x4)

Creates an affine transform from the specified 4 x 4 double-precision matrix.

Deprecated

init?(matrix: simd_double4x4)

Creates an affine transform from the specified 4 x 4 double-precision matrix.

Deprecated

init(matrix: simd_float4x3)

Creates an affine transform from the specified single-precision matrix.

Deprecated

init?(matrix: simd_float4x4)

Creates an affine transform from the specified 4 x 4 single-precision matrix.

Deprecated

init?(projectiveTransform: ProjectiveTransform3D)

Creates an affine transform from the specified projective transform.

Deprecated

init(scale: Size3D, rotation: Rotation3D, translation: Size3D)

Creates an affine transform from the specified scale, rotate, and translate transforms.

Deprecated

init(translation: Size3D)Deprecated

func inverted() -> AffineTransform3D?

Returns a new transform that results from inverting an existing affine transform.

Deprecated

