

- RealityKit
- MeshResource
- MeshResource.Skeleton
- MeshResource.Skeleton.Joint
-  parentIndex 

Instance Property

# parentIndex

The index of this joint’s parent, or nil if this joint has no parent.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var parentIndex: Int?
```

## Discussion

If the joint has a parent, the index of the parent needs to be lower than that of the child.

