

- RealityKit
- Entity
- Entity.ChildCollection
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Adds the specified list of entity as children to this entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func append(contentsOf sequence: S) where S : Sequence, S.Element : Entity
```

## Parameters 

`sequence`  

The child entities to add to the collection.

