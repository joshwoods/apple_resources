

- Swift
- String
- Substring
-  BidirectionalCollection Implementations 

API Collection

# BidirectionalCollection Implementations

## Topics

### Instance Properties

var last: Self.Element?

The last element of the collection.

### Instance Methods

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: Substring.Index, to: Substring.Index) -> Int

Returns the distance between two indices.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func index(Substring.Index, offsetBy: Int) -> Substring.Index

Returns an index that is the specified distance from the given index.

func index(Substring.Index, offsetBy: Int, limitedBy: Substring.Index) -> Substring.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: Substring.Index) -> Substring.Index

Returns the position immediately after the given index.

func index(before: Substring.Index) -> Substring.Index

Returns the position immediately before the given index.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the given number of elements from the end of the collection.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

### Subscripts

subscript(Range&lt;Substring.Index>) -> Substring

Accesses a contiguous subrange of the collection’s elements.

