

- ARKit
- ARSkeleton2D
-  jointLandmarks 

Instance Property

# jointLandmarks

The joint landmarks in normalized coordinates.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
var jointLandmarks: [simd_float2] { get }
```

## Discussion

The joint landmarks are normalized within the range \[0..1\] in the coordinate space of the current frame’s camera image, where 0 is the upper left, and 1 is the bottom right.

## See Also

### Getting Joint Landmarks

func landmark(for: ARSkeleton.JointName) -> simd_float2?

Returns the location of a joint with a given name.

