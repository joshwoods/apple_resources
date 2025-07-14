

- RealityKit
- MeshResource
- MeshResource.Skeleton
- MeshResource.Skeleton.Joint
-  restPoseTransform 

Instance Property

# restPoseTransform

The local transform of this joint in skeleton’s rest pose, specified relative to this joint’s parent (or relative to model space, if this joint has no parent).

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var restPoseTransform: Transform
```

## Discussion

The rest pose of a skeleton is used when a joint is not otherwise animated.

