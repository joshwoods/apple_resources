

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- AnyCollection
-  Collection Implementations 

API Collection

# Collection Implementations

## Topics

### Instance Properties

var count: Int

The number of elements.

var endIndex: AnyCollection&lt;Element>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var first: Self.Element?

The first element of the collection.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: AnyCollection&lt;Element>.Index

The position of the first element in a non-empty collection.

### Instance Methods

func distance(from: AnyCollection&lt;Element>.Index, to: AnyCollection&lt;Element>.Index) -> Int

Returns the distance between two indices.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func formIndex(after: inout AnyCollection&lt;Element>.Index)

Replaces the given index with its successor.

func index(AnyCollection&lt;Element>.Index, offsetBy: Int) -> AnyCollection&lt;Element>.Index

Returns an index that is the specified distance from the given index.

func index(AnyCollection&lt;Element>.Index, offsetBy: Int, limitedBy: AnyCollection&lt;Element>.Index) -> AnyCollection&lt;Element>.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: AnyCollection&lt;Element>.Index) -> AnyCollection&lt;Element>.Index

Returns the position immediately after the given index.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func indices(of: Self.Element) -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that are equal to the given element.

func indices(where: (Self.Element) throws -> Bool) rethrows -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that match the given predicate.

func makeIterator() -> AnyCollection&lt;Element>.Iterator

Returns an iterator over the elements of this collection.

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func popFirst() -> Self.Element?

Removes and returns the first element of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

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

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

### Subscripts

subscript(RangeSet&lt;Self.Index>) -> DiscontiguousSlice&lt;Self>

Accesses a view of this collection with the elements at the given indices.

subscript(AnyCollection&lt;Element>.Index) -> Element

Accesses the element indicated by `position`.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript(Range&lt;AnyCollection&lt;Element>.Index>) -> AnyCollection&lt;Element>.SubSequence

Accesses a contiguous subrange of the collection’s elements.

### Type Aliases

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

