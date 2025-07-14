

- RealityKit
- Entity
- Entity.ChildCollection
-  firstRange(of:) 

Instance Method

# firstRange(of:)

Finds and returns the range of the first occurrence of a given collection within this collection.

RealityKitSwiftiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func firstRange(of other: C) -> Range? where C : Collection, Self.Element == C.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

The collection to search for.

## Return Value

A range in the collection of the first occurrence of `sequence`. Returns nil if `sequence` is not found.

