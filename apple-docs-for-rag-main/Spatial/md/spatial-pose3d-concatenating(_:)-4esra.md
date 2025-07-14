

- Spatial
- Pose3D
-  concatenating(\_:) 

Instance Method

# concatenating(\_:)

Returns a pose that represents the concatenation of a scaled pose and a pose.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func concatenating(_ transform: ScaledPose3D) -> ScaledPose3D
```

## See Also

### Transforming a 3D pose structure

func concatenating(Pose3D) -> Pose3D

Returns a pose that represents the concatenation of two poses.

func flip(along: Axis3D)

Flips a pose along the specified axis.

func flipped(along: Axis3D) -> Pose3D

Returns a pose that results from flipping it along the specified axis.

func rotated(by: simd_quatd) -> Pose3D

Returns a pose that results from rotating with the specified quaternion.

func rotated(by: Rotation3D) -> Pose3D

Returns a pose that results from applying the specified rotation.

