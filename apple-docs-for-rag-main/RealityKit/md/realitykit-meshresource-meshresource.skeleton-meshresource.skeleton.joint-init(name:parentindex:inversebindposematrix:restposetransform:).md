

- RealityKit
- MeshResource
- MeshResource.Skeleton
- MeshResource.Skeleton.Joint
-  init(name:parentIndex:inverseBindPoseMatrix:restPoseTransform:) 

Initializer

# init(name:parentIndex:inverseBindPoseMatrix:restPoseTransform:)

Creates a single joint in a skeleton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    name: String,
    parentIndex: Int?,
    inverseBindPoseMatrix: simd_float4x4,
    restPoseTransform: Transform
)
```

