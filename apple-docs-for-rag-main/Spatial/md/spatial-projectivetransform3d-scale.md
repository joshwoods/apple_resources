

- Spatial
- ProjectiveTransform3D
-  scale 

Instance Property

# scale

The projective transform’s scale.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Mac Catalyst

``` source
var scale: Size3D? { get }
```

## See Also

### Deprecated symbols

var offset: Vector3D

The projective transform’s translation.

Deprecated

func inverted() -> ProjectiveTransform3D?

Returns a new transform that results from inverting an existing projective transform.

Deprecated

init(matrix: simd_float4x4)

Creates a projective transform from the specified 4 x 4 single-precision matrix.

Deprecated

init(scale: Size3D, rotation: Rotation3D, translation: Size3D)

Creates a projective transform from the specified scale, rotate, and translate transforms.

Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform with right-hand-side perspective and optional reverse-z.

Deprecated

init(translation: Size3D)Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double)Deprecated

