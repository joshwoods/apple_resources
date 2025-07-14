

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the entity from the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
mutating func remove(_ child: Entity)
```

## Discussion

Note

This operation can invalidate the index order of any remaining entities.

