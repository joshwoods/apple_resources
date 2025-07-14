

- RealityKit
- EntityCollection
-  removeAll(where:) 

Instance Method

# removeAll(where:)

Removes all entities from this collection that satisfy the given predicate.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func removeAll(where: (Entity) throws -> Bool) rethrows
```

**Required** Default implementation provided.

## Discussion

Note

This operation can invalidate the index order of any remaining entities.

## Default Implementations

### EntityCollection Implementations

func removeAll(where: (Entity) throws -> Bool) rethrows

Removes all entities from this collection that satisfy the given predicate.

