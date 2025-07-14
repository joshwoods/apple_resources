

- ARKit
- HandSkeleton
- HandSkeleton.Joint
-  isTracked 

Instance Property

# isTracked

A Boolean value that indicates whether ARKit is currently tracking this joint.

visionOS 1.0+

``` source
var isTracked: Bool { get }
```

## See Also

### Tracking the position of hand joints

var anchorFromJointTransform: simd_float4x4

The position and orientation of this joint relative to the base joint of the skeleton.

var parentFromJointTransform: simd_float4x4

The transform from the joint to its parent joint’s coordinate system.

