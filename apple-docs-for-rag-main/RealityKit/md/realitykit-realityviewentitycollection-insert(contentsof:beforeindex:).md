

- RealityKit
- RealityViewEntityCollection
-  insert(contentsOf:beforeIndex:) 

Instance Method

# insert(contentsOf:beforeIndex:)

Adds the specified sequence of entities to this collection in order, directly before the entity at the given index.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func insert(
    contentsOf sequence: S,
    beforeIndex index: Int
) where S : Sequence, S.Element : Entity
```

## Parameters 

`sequence`  

A sequence of entities to add to the collection.

`index`  

The index of an entity to insert in front of. If `endIndex` is provided, the entities will be appended.

## Discussion

Note

This operation can invalidate the index order of any extant entities.

