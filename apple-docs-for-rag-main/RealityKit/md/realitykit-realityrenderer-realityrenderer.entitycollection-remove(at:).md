

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  remove(at:) 

Instance Method

# remove(at:)

Removes the entity at the given index from this collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
mutating func remove(at index: Int)
```

## Parameters 

`index`  

The index of the entity to remove from the collection.

## Discussion

Note

This operation can invalidate the index order of any remaining entities.

