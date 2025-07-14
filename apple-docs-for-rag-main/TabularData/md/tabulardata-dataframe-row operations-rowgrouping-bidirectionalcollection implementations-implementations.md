

- TabularData
- DataFrame
- Row Operations
- RowGrouping
-  BidirectionalCollection Implementations 

API Collection

# BidirectionalCollection Implementations

## Topics

### Instance Properties

var last: Self.Element?

The last element of the collection.

### Instance Methods

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

