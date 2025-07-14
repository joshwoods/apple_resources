

- Spatial
- ScaledPose3D
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Returns the concatenation of a pose and a scaled pose.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
static func * (lhs: Pose3D, rhs: ScaledPose3D) -> ScaledPose3D
```

## See Also

### Applying arithmetic operations

static func * (ScaledPose3D, ScaledPose3D) -> ScaledPose3D

Returns the concatenation of two scaled poses.

static func * (ScaledPose3D, Pose3D) -> ScaledPose3D

Returns the concatenation of a scaled pose and a pose.

static func *= (inout ScaledPose3D, ScaledPose3D)

Concatenates two scaled poses and stores the result in the left-hand-side variable.

