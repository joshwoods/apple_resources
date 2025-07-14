

- ARKit
- HandSkeleton
- HandSkeleton.Joint
-  anchorFromJointTransform 

Instance Property

# anchorFromJointTransform

The position and orientation of this joint relative to the base joint of the skeleton.

visionOS 1.0+

``` source
var anchorFromJointTransform: simd_float4x4 { get }
```

## See Also

### Tracking the position of hand joints

var parentFromJointTransform: simd_float4x4

The transform from the joint to its parent joint’s coordinate system.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this joint.

