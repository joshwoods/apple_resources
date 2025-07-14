

- Spatial
- Vector3D
-  applying(\_:) 

Instance Method

# applying(\_:)

Returns the vector resulting from applying an affine transform to the vector.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applying(_ transform: AffineTransform3D) -> Vector3D
```

## Parameters 

`transform`  

The affine transform.

## Discussion

- Returns The transformed primitive.

## See Also

### Transforming a vector

func applying(ProjectiveTransform3D) -> Vector3D

Returns the vector resulting from applying a projective transform to the vector.

func applying(Pose3D) -> Vector3D

Returns a vector that results from applying the specified pose.

func unapplying(AffineTransform3D) -> Vector3D

Returns the vector resulting from unapplying an affine transform to the vector.

func unapplying(ProjectiveTransform3D) -> Vector3D

Returns the vector resulting from unapplying a projective transform to the vector.

func unapplying(Pose3D) -> Vector3D

Returns a vector that results from unapplying the specified pose.

func rotated(by: Rotation3D) -> Vector3D

Returns the vector rotated by the specified rotation around the origin.

func rotated(by: simd_quatd) -> Vector3D

Returns the vector rotated by the specified quaternion around the origin.

func scaled(by: Size3D) -> Vector3D

Returns the vector scaled by the specified size.

func scaledBy(x: Double, y: Double, z: Double) -> Vector3D

Returns a vector that results from scaling with the specified double-precision values.

func uniformlyScaled(by: Double) -> Vector3D

Returns the entity uniformly scaled by the specified scalar value.

func sheared(AxisWithFactors) -> Vector3D

Returns a vector that results from shearing over an axis by shear factors for the other two axes.

func applying(ScaledPose3D) -> Vector3D

Returns a vector that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Vector3D

Returns a vector that’s transformed by the inverse of the specified scaled pose.

