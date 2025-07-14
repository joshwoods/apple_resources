

- Spatial
- ScaledPose3D
-  isApproximatelyEqual(to:tolerance:) 

Instance Method

# isApproximatelyEqual(to:tolerance:)

Returns a Boolean value that indicates whether two scaled poses are equal within a specified tolerance.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func isApproximatelyEqual(
    to other: ScaledPose3D,
    tolerance: Double = sqrt(.ulpOfOne)
) -> Bool
```

## See Also

### Comparing values

static func == (ScaledPose3D, ScaledPose3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

