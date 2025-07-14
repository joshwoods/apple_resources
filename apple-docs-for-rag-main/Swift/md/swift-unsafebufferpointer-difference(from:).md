

- Swift
- UnsafeBufferPointer
-  difference(from:) 

Instance Method

# difference(from:)

Returns the difference needed to produce this collection’s ordered elements from the given collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func difference(from other: C) -> CollectionDifference where C : BidirectionalCollection, Self.Element == C.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

The base state.

## Return Value

The difference needed to produce this collection’s ordered elements from the given collection.

## Discussion

This function does not infer element moves. If you need to infer moves, call the `inferringMoves()` method on the resulting difference.

Complexity

Worst case performance is O(*n* \* *m*), where *n* is the count of this collection and *m* is `other.count`. You can expect faster execution when the collections share many common elements, or if `Element` conforms to `Hashable`.

