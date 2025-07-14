

- RealityKit
- MeshResource
- MeshResource.Skeleton
-  joints 

Instance Property

# joints

The joints which define this skeleton’s hierarchy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var joints: [MeshResource.Skeleton.Joint]
```

## Discussion

Important

The order of joints in this array is significant; parents need to precede their children.

