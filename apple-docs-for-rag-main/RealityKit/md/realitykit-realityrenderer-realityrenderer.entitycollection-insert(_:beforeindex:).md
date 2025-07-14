

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  insert(\_:beforeIndex:) 

Instance Method

# insert(\_:beforeIndex:)

Adds the specified entity to this collection directly before the entity at the given index. If the entity is already located before the index, the collection will not change.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func insert(
    _ entity: Entity,
    beforeIndex index: Int
)
```

## Parameters 

`entity`  

The entity to add to the collection.

`index`  

The index of an entity to insert in front of. If `endIndex` is provided, the entity will be appended.

## Discussion

Note

This operation can invalidate the index order of any extant entities.

