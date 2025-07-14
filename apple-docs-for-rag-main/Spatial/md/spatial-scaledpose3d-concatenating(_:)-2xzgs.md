

- Spatial
- ScaledPose3D
-  concatenating(\_:) 

Instance Method

# concatenating(\_:)

Returns a scaled pose that represents the concatenation of two poses.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func concatenating(_ transform: Pose3D) -> ScaledPose3D
```

## See Also

### Transforming a 3D scaled-pose structure

func flip(along: Axis3D)

Flips a scaled pose along the specified axis.

func flipped(along: Axis3D) -> ScaledPose3D

Returns a scaled pose that results from flipping it along the specified axis.

func rotated(by: simd_quatd) -> ScaledPose3D

Returns a scaled pose that results from rotating with the specified quaternion.

func rotated(by: Rotation3D) -> ScaledPose3D

Returns a scaled pose that results from applying the specified rotation.

func concatenating(ScaledPose3D) -> ScaledPose3D

Returns a scaled pose that represents the concatenation of two scaled poses.

