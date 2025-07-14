

- RealityKit
- EntityCollection
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Adds the specified sequence of entities to the end of this collection, in order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func append(contentsOf sequence: S) where S : Sequence, S.Element : Entity
```

**Required** Default implementation provided.

## Parameters 

`sequence`  

The entities to add to the collection.

## Discussion

Note

This operation can invalidate the index order of any extant entities.

## Default Implementations

### EntityCollection Implementations

func append&lt;S>(contentsOf: S)

Adds the specified sequence of entities to the end of this collection, in order.

