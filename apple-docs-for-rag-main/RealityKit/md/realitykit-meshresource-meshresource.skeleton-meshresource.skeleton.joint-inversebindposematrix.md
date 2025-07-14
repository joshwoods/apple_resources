

- RealityKit
- MeshResource
- MeshResource.Skeleton
- MeshResource.Skeleton.Joint
-  inverseBindPoseMatrix 

Instance Property

# inverseBindPoseMatrix

A matrix which transforms from the authored pose (the “bind pose”) of the bound model to the local space of this joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var inverseBindPoseMatrix: simd_float4x4
```

## Discussion

Note

The bind pose matrix transforms a vertex from a joint’s local coordinate space to the position of that vertex in the model’s bind pose. This property is the *inverse* bind pose matrix, so it transforms a vertex from its position in the model’s bind pose to the local coordinate space of this joint.

