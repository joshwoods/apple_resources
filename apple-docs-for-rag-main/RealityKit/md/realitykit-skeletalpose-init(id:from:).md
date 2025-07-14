

- RealityKit
- SkeletalPose
-  init(id:from:) 

Initializer

# init(id:from:)

Creates a skeletal pose from the rest pose of the model skeleton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    id: SkeletalPose.ID,
    from skeleton: MeshResource.Skeleton
)
```

## Parameters 

`id`  

The unique name of the pose.

`skeleton`  

The skeleton to extract the joint names and rest pose transformations from.

