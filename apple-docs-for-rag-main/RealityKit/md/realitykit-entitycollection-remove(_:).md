

- RealityKit
- EntityCollection
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the entity from the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func remove(_ entity: Entity)
```

**Required** Default implementation provided.

## Parameters 

`entity`  

The entity to remove from the collection.

## Discussion

Note

This operation can invalidate the index order of any remaining entities.

## Default Implementations

### EntityCollection Implementations

func remove(Entity)

Removes the entity from the collection.

