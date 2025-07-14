

- Spatial
- AffineTransform3D
-  init(scale:rotation:translation:) Deprecated

Initializer

# init(scale:rotation:translation:)

Creates an affine transform from the specified scale, rotate, and translate transforms.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+visionOS

``` source
init(
    scale: Size3D = Size3D(width: 1.0, height: 1, depth: 1),
    rotation: Rotation3D = .zero,
    translation: Size3D
)
```

Deprecated

Use `Vector3D` variant.

## Parameters 

`scale`  

A size structure that specifies the scale.

`rotation`  

A rotation structure that specifies the rotation.

`translation`  

A size structure that specifies the translation.

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

init(translation: Size3D)Deprecated

func inverted() -> AffineTransform3D?

Returns a new transform that results from inverting an existing affine transform.

Deprecated

var offset: Vector3D

The affine transform’s translation.

Deprecated

