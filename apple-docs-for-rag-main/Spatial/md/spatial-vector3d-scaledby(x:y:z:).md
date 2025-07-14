

- Spatial
- Vector3D
-  scaledBy(x:y:z:) 

Instance Method

# scaledBy(x:y:z:)

Returns a vector that results from scaling with the specified double-precision values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func scaledBy(
    x: Double = 1,
    y: Double = 1,
    z: Double = 1
) -> Vector3D
```

## Parameters 

`x`  

The double-precision value that specifies the scale for the x-element.

`y`  

The double-precision value that specifies the scale for the y-element.

`z`  

The double-precision value that specifies the scale for the z-element.

## Return Value

The vector that results from scaling with the specified double-precision values.

## See Also

### Transforming a vector

func applying(AffineTransform3D) -> Vector3D

Returns the vector resulting from applying an affine transform to the vector.

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

func uniformlyScaled(by: Double) -> Vector3D

Returns the entity uniformly scaled by the specified scalar value.

func sheared(AxisWithFactors) -> Vector3D

Returns a vector that results from shearing over an axis by shear factors for the other two axes.

func applying(ScaledPose3D) -> Vector3D

Returns a vector that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Vector3D

Returns a vector that’s transformed by the inverse of the specified scaled pose.

