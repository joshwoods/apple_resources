

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  replaceAll(\_:) 

Instance Method

# replaceAll(\_:)

Replaces all entities in this collection with those from the given sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
mutating func replaceAll(_ entities: S) where S : Sequence, S.Element : Entity
```

## Parameters 

`entities`  

The sequence of entities that will replace the collection’s current contents.

## Discussion

Note

This operation might not maintain the new entities’ index order.

