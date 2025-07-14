

- TabularData
- Column
-  BidirectionalCollection Implementations 

API Collection

# BidirectionalCollection Implementations

## Topics

### Instance Properties

var endIndex: Int

The index of the final element in the column.

var last: Self.Element?

The last element of the collection.

var startIndex: Int

The index of the initial element in the column.

### Instance Methods

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: Self.Index, to: Self.Index) -> Int

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func index(Self.Index, offsetBy: Int) -> Self.Index

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(before: Int) -> Int

Returns the index immediately before an element index.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

### Subscripts

subscript(Range&lt;Int>) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

subscript(Int) -> Column&lt;WrappedElement>.Element

Accesses an element at an index.

