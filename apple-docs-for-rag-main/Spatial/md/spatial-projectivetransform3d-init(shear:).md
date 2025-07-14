

- Spatial
- ProjectiveTransform3D
-  init(shear:) 

Initializer

# init(shear:)

Creates a projective transform from the specified shear transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(shear: AxisWithFactors)
```

## Parameters 

`shear`  

The shear axis and factors.

## See Also

### Creating a 3D projective transform structure

init()

Creates a projective transform.

init()

Returns a new identity projective transform.

init(simd_float4x4)

Creates a projective transform from the specified 4 x 4 single-precision matrix.

init(simd_double4x4)

Creates a projective transform from the specified double-precision matrix.

init(matrix: simd_double4x4)

Creates a projective transform from the specified 4 x 4 double-precision matrix.

init(AffineTransform3D)

Creates a projective transform from the specified affine transform.

init(pose: Pose3D)

Creates a projective transform from the specified pose structure.

init(scale: Size3D, rotation: Rotation3D, translation: Vector3D)

Creates a projective transform from the specified scale, rotate, and translate transforms.

init(scale: Size3D)

Creates a projective transform from the specified scale transform.

init(rotation: Rotation3D)

Creates a projective transform from the specified rotate transform.

init(translation: Vector3D)

Creates a projective transform from the specified translate transform.

init(leftTangent: Double, rightTangent: Double, topTangent: Double, bottomTangent: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform from tangents for each side of its frustum.

init(fovY: Angle2D, aspectRatio: Double, nearZ: Double, farZ: Double)

Returns a projective transform with right-hand side perspective.

init(fovY: Angle2D, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

init(scaledPose: ScaledPose3D)

