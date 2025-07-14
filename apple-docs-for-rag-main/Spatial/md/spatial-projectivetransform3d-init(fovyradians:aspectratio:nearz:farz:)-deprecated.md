

- Spatial
- ProjectiveTransform3D
-  init(fovyRadians:aspectRatio:nearZ:farZ:) Deprecated

Initializer

# init(fovyRadians:aspectRatio:nearZ:farZ:)

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
init(
    fovyRadians: Double,
    aspectRatio: Double,
    nearZ: Double,
    farZ: Double
)
```

Deprecated

Use \`SPAngle\` variant of \`SPProjectiveTransform3DMakeWithRightHandPerspective\`.

## Parameters 

`fovyRadians`  

The field of view angle on the @p y axis.

`aspectRatio`  

The aspect ratio.

`nearZ`  

The near @p z .

`farZ`  

The far @p z .

## Return Value

A projective transform with right-hand side perspective.

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

init(scale: Size3D, rotation: Rotation3D, translation: Size3D)

Creates a projective transform from the specified scale, rotate, and translate transforms.

Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform with right-hand-side perspective and optional reverse-z.

Deprecated

init(translation: Size3D)Deprecated

