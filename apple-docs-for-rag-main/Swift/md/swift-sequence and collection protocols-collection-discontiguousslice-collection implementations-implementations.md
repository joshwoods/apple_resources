

- Swift
- Swift Standard Library
- Collections
- 
  - Swift Standard Library
  - Collections
- Sequence and Collection Protocols
- Collection
- DiscontiguousSlice
-  Collection Implementations 

API Collection

# Collection Implementations

## Topics

### Structures

struct Index

A position in a `DiscontiguousSlice`.

### Instance Properties

var count: Int

The number of elements in the collection.

var count: Int

The number of elements in the collection.

var endIndex: DiscontiguousSlice&lt;Base>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var first: Self.Element?

The first element of the collection.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: DiscontiguousSlice&lt;Base>.Index

The position of the first element in a nonempty collection.

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

### Instance Methods

func distance(from: DiscontiguousSlice&lt;Base>.Index, to: DiscontiguousSlice&lt;Base>.Index) -> Int

Returns the distance between two indices.

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: DiscontiguousSlice&lt;Base>.Index) -> DiscontiguousSlice&lt;Base>.Index

Returns the position immediately after the given index.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func indices(of: Self.Element) -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that are equal to the given element.

func indices(where: (Self.Element) throws -> Bool) rethrows -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that match the given predicate.

func makeIterator() -> IndexingIterator&lt;Self>

Returns an iterator over the elements of the collection.

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func popFirst() -> Self.Element?

Removes and returns the first element of the collection.

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

func removingSubranges(RangeSet&lt;Self.Index>) -> DiscontiguousSlice&lt;Self>

Returns a collection of the elements in this collection that are not represented by the given range set.

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, that don’t contain elements satisfying the given predicate.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

### Subscripts

subscript(Range&lt;DiscontiguousSlice&lt;Base>.Index>) -> DiscontiguousSlice&lt;Base>

Accesses a contiguous subrange of the collection’s elements.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript(DiscontiguousSlice&lt;Base>.Index) -> Base.Element

Accesses the element at the specified position.

### Type Aliases

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

