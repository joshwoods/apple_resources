

- Spatial
- ProjectiveTransform3D
-  init(scale:rotation:translation:) Deprecated

Initializer

# init(scale:rotation:translation:)

Creates a projective transform from the specified scale, rotate, and translate transforms.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

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

var offset: Vector3D

The projective transform’s translation.

Deprecated

var scale: Size3D?

The projective transform’s scale.

Deprecated

func inverted() -> ProjectiveTransform3D?

Returns a new transform that results from inverting an existing projective transform.

Deprecated

init(matrix: simd_float4x4)

Creates a projective transform from the specified 4 x 4 single-precision matrix.

Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform with right-hand-side perspective and optional reverse-z.

Deprecated

init(translation: Size3D)Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double)Deprecated

