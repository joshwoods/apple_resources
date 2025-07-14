

- RealityKit
- MeshResource
- MeshResource.Skeleton
-  init(id:joints:) 

Initializer

# init(id:joints:)

Creates a skeleton from an array of joints.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    id: String,
    joints: [MeshResource.Skeleton.Joint]
)
```

## Discussion

Important

The order of joints in this array is significant; parents need to precede their children.

