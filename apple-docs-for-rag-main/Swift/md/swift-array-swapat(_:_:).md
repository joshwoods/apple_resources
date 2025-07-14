

- Swift
- Array
-  swapAt(\_:\_:) 

Instance Method

# swapAt(\_:\_:)

Exchanges the values at the specified indices of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func swapAt(
    _ i: Self.Index,
    _ j: Self.Index
)
```

## Parameters 

`i`  

The index of the first value to swap.

`j`  

The index of the second value to swap.

## Discussion

Both parameters must be valid indices of the collection that are not equal to `endIndex`. Calling `swapAt(_:_:)` with the same index as both `i` and `j` has no effect.

Complexity

O(1)

## See Also

### Reordering an Array’s Elements

func sort()

Sorts the collection in place.

func sort(by: (Self.Element, Self.Element) throws -> Bool) rethrows

Sorts the collection in place, using the given predicate as the comparison between elements.

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func reverse()

Reverses the elements of the collection in place.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func shuffle()

Shuffles the collection in place.

func shuffle&lt;T>(using: inout T)

Shuffles the collection in place, using the given generator as a source for randomness.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

func partition(by: (Self.Element) throws -> Bool) rethrows -> Self.Index

Reorders the elements of the collection such that all the elements that match the given predicate are after all the elements that don’t match.

