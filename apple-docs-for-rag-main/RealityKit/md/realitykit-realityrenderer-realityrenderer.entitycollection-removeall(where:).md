

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  removeAll(where:) 

Instance Method

# removeAll(where:)

Removes all entities from this collection that satisfy the given predicate.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func removeAll(where shouldBeRemoved: (Entity) throws -> Bool) rethrows
```

## Discussion

Note

This operation can invalidate the index order of any remaining entities.

