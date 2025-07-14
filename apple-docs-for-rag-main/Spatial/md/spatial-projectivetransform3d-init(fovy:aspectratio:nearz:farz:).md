

- Spatial
- ProjectiveTransform3D
-  init(fovY:aspectRatio:nearZ:farZ:) 

Initializer

# init(fovY:aspectRatio:nearZ:farZ:)

Returns a projective transform with right-hand side perspective.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    fovY: Angle2D,
    aspectRatio: Double,
    nearZ: Double,
    farZ: Double
)
```

## Discussion

- fovyRadians: The field-of-view angle along the y-axis.

- aspectRatio: The aspect ratio.

- nearZ: The distance to the near clipping plane.

- farZ: The distance to the far clipping plane.

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

init(shear: AxisWithFactors)

Creates a projective transform from the specified shear transform.

init(leftTangent: Double, rightTangent: Double, topTangent: Double, bottomTangent: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform from tangents for each side of its frustum.

init(fovY: Angle2D, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

init(scaledPose: ScaledPose3D)

