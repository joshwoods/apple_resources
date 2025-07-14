

- Swift
- Swift Standard Library
- Manual Memory Management
- UnsafeMutableRawBufferPointer
-  Collection Implementations 

API Collection

# Collection Implementations

## Topics

### Instance Properties

var count: Int

The number of bytes in the buffer.

var endIndex: UnsafeMutableRawBufferPointer.Index

The “past the end” position—that is, the position one greater than the last valid subscript argument.

var first: Self.Element?

The first element of the collection.

var indices: UnsafeMutableRawBufferPointer.Indices

The indices that are valid for subscripting the collection, in ascending order.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: UnsafeMutableRawBufferPointer.Index

Always zero, which is the index of the first byte in a nonempty buffer.

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

### Instance Methods

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

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

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func indices(of: Self.Element) -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that are equal to the given element.

func indices(where: (Self.Element) throws -> Bool) rethrows -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that match the given predicate.

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

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

func removingSubranges(RangeSet&lt;Self.Index>) -> DiscontiguousSlice&lt;Self>

Returns a collection of the elements in this collection that are not represented by the given range set.

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, that don’t contain elements satisfying the given predicate.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

### Subscripts

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

subscript(RangeSet&lt;Self.Index>) -> DiscontiguousSlice&lt;Self>

Accesses a view of this collection with the elements at the given indices.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

### Type Aliases

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

