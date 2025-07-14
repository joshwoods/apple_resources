

- RealityKit
- Entity
- Entity.ChildCollection
-  replaceAll(\_:) 

Instance Method

# replaceAll(\_:)

Removes all children from this entity and adds the specified list of entities as the new children.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func replaceAll(_ children: S) where S : Sequence, S.Element : Entity
```

## Parameters 

`children`  

The list of the new children.

