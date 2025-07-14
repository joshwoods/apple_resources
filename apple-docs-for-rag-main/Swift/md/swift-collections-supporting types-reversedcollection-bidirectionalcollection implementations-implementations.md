

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- ReversedCollection
-  BidirectionalCollection Implementations 

API Collection

# BidirectionalCollection Implementations

## Topics

### Structures

struct Index

An index that traverses the same positions as an underlying index, with inverted traversal direction.

### Instance Properties

var last: Self.Element?

The last element of the collection.

### Instance Methods

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: ReversedCollection&lt;Base>.Index, to: ReversedCollection&lt;Base>.Index) -> Int

Returns the distance between two indices.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func index(ReversedCollection&lt;Base>.Index, offsetBy: Int) -> ReversedCollection&lt;Base>.Index

Returns an index that is the specified distance from the given index.

func index(ReversedCollection&lt;Base>.Index, offsetBy: Int, limitedBy: ReversedCollection&lt;Base>.Index) -> ReversedCollection&lt;Base>.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: ReversedCollection&lt;Base>.Index) -> ReversedCollection&lt;Base>.Index

Returns the position immediately after the given index.

func index(before: ReversedCollection&lt;Base>.Index) -> ReversedCollection&lt;Base>.Index

Returns the position immediately before the given index.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

