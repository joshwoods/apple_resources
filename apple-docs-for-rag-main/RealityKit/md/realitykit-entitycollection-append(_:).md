

- RealityKit
- EntityCollection
-  append(\_:) 

Instance Method

# append(\_:)

Adds the specified entity to the end of this collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func append(_ entity: Entity)
```

**Required** Default implementation provided.

## Parameters 

`entity`  

The entity to add to the collection.

## Discussion

Note

This operation can invalidate the index order of any extant entities.

## Default Implementations

### EntityCollection Implementations

func append(Entity)

Adds the specified entity to the end of this collection.

