

- ARKit
- ARSkeleton2D
-  landmark(for:) 

Instance Method

# landmark(for:)

Returns the location of a joint with a given name.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
func landmark(for jointName: ARSkeleton.JointName) -> simd_float2?
```

## Discussion

Joint landmarks are normalized within the range \[0..1\] and are in the coordinate space of the current frame’s camera image, where 0 is the upper left, and 1 is the bottom right.

## See Also

### Getting Joint Landmarks

var jointLandmarks: [simd_float2]

The joint landmarks in normalized coordinates.

