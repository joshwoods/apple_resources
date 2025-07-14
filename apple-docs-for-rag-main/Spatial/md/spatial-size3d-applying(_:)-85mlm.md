

- Spatial
- Size3D
-  applying(\_:) 

Instance Method

# applying(\_:)

Returns a size that results from applying the specified pose.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applying(_ pose: Pose3D) -> Size3D
```

## Parameters 

`pose`  

The pose that the function applies to the size.

## See Also

### Transforming a 3D size structure

func applying(ScaledPose3D) -> Size3D

Returns a size that’s transformed by the specified scaled pose.

func unapplying(AffineTransform3D) -> Size3D

Returns a size that results from unapplying the specified affine transform.

func unapplying(ProjectiveTransform3D) -> Size3D

Returns a size that results from unapplying the specified projective transform.

func unapplying(Pose3D) -> Size3D

Returns a size that results from unapplying the specified pose.

func sheared(AxisWithFactors) -> Size3D

Returns a size that results from shearing over an axis by shear factors for the other two axes.

func applying(ScaledPose3D) -> Size3D

Returns a size that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Size3D

Returns a size that’s transformed by the inverse of the specified scaled pose.

