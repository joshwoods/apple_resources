

- RealityKit
- Entity
- Entity.ComponentSet
-  distance(from:to:) 

Instance Method

# distance(from:to:)

Returns the distance between two indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
func distance(
    from start: Entity.ComponentSet.Index,
    to end: Entity.ComponentSet.Index
) -> Int
```

## Parameters 

`start`  

A valid index of the collection.

`end`  

Another valid index of the collection. If `end` is equal to `start`, the result is zero.

## Return Value

The distance between `start` and `end`. The result can be negative only if the collection conforms to the `BidirectionalCollection` protocol.

## Discussion

Unless the collection conforms to the `BidirectionalCollection` protocol, `start` must be less than or equal to `end`.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the resulting distance.

