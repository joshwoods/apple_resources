

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- AnyBidirectionalCollection
-  BidirectionalCollection Implementations 

API Collection

# BidirectionalCollection Implementations

## Topics

### Instance Properties

var endIndex: AnyBidirectionalCollection&lt;Element>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var last: Self.Element?

The last element of the collection.

var startIndex: AnyBidirectionalCollection&lt;Element>.Index

The position of the first element in a non-empty collection.

### Instance Methods

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: AnyBidirectionalCollection&lt;Element>.Index, to: AnyBidirectionalCollection&lt;Element>.Index) -> Int

Returns the distance between two indices.

func formIndex(after: inout AnyBidirectionalCollection&lt;Element>.Index)

Replaces the given index with its successor.

func formIndex(before: inout AnyBidirectionalCollection&lt;Element>.Index)

Replaces the given index with its predecessor.

func index(AnyBidirectionalCollection&lt;Element>.Index, offsetBy: Int) -> AnyBidirectionalCollection&lt;Element>.Index

Returns an index that is the specified distance from the given index.

func index(AnyBidirectionalCollection&lt;Element>.Index, offsetBy: Int, limitedBy: AnyBidirectionalCollection&lt;Element>.Index) -> AnyBidirectionalCollection&lt;Element>.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: AnyBidirectionalCollection&lt;Element>.Index) -> AnyBidirectionalCollection&lt;Element>.Index

Returns the position immediately after the given index.

func index(before: AnyBidirectionalCollection&lt;Element>.Index) -> AnyBidirectionalCollection&lt;Element>.Index

Returns the position immediately before the given index.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

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

### Subscripts

subscript(AnyBidirectionalCollection&lt;Element>.Index) -> Element

Accesses the element indicated by `position`.

subscript(Range&lt;AnyBidirectionalCollection&lt;Element>.Index>) -> AnyBidirectionalCollection&lt;Element>.SubSequence

Accesses a contiguous subrange of the collection’s elements.

