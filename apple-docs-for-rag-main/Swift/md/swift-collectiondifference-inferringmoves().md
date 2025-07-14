

- Swift
- CollectionDifference
-  inferringMoves() 

Instance Method

# inferringMoves()

Returns a new collection difference with associations between individual elements that have been removed and inserted only once.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func inferringMoves() -> CollectionDifference
```

Available when `ChangeElement` conforms to `Hashable`.

## Return Value

A collection difference with all possible moves inferred.

## Discussion

Complexity

O(*n*) where *n* is the number of collection differences.

