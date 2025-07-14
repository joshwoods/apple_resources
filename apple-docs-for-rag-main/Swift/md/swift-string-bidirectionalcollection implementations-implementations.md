

- Swift
- String
-  BidirectionalCollection Implementations 

API Collection

# BidirectionalCollection Implementations

## Topics

### Structures

struct Index

A position of a character or code unit in a string.

### Instance Properties

var endIndex: String.Index

A string’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var last: Self.Element?

The last element of the collection.

var startIndex: String.Index

The position of the first character in a nonempty string.

### Instance Methods

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: String.Index, to: String.Index) -> Int

Returns the distance between two indices.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func index(String.Index, offsetBy: Int) -> String.Index

Returns an index that is the specified distance from the given index.

func index(String.Index, offsetBy: Int, limitedBy: String.Index) -> String.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: String.Index) -> String.Index

Returns the position immediately after the given index.

func index(before: String.Index) -> String.Index

Returns the position immediately before the given index.

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

subscript(Range&lt;String.Index>) -> Substring

Accesses a contiguous subrange of the collection’s elements.

subscript(String.Index) -> Character

Accesses the character at the given position.

