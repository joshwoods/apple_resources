

- ARKit
- HandSkeleton
- HandSkeleton.Joint
-  parentFromJointTransform 

Instance Property

# parentFromJointTransform

The transform from the joint to its parent joint’s coordinate system.

visionOS 1.0+

``` source
var parentFromJointTransform: simd_float4x4 { get }
```

## Discussion

The root joint’s parentFromJointTransform is an identity matrix.

## See Also

### Tracking the position of hand joints

var anchorFromJointTransform: simd_float4x4

The position and orientation of this joint relative to the base joint of the skeleton.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this joint.

