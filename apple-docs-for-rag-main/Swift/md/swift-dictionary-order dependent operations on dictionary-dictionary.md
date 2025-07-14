

- Swift
- Dictionary
-  Order Dependent Operations on Dictionary 

API Collection

# Order Dependent Operations on Dictionary

Perform order-dependent operations common to all collections, as implemented for `Dictionary`.

## Topics

### Comparing Dictionaries

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

### Manipulating Indices

var startIndex: Dictionary&lt;Key, Value>.Index

The position of the first element in a nonempty dictionary.

var endIndex: Dictionary&lt;Key, Value>.Index

The dictionary’s “past the end” position—that is, the position one greater than the last valid subscript argument.

func index(after: Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Index

Returns the position immediately after the given index.

func formIndex(after: inout Dictionary&lt;Key, Value>.Index)

Replaces the given index with its successor.

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

### Selecting Elements

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

### Excluding Elements

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func popFirst() -> Dictionary&lt;Key, Value>.Element?

Removes and returns the first key-value pair of the dictionary if the dictionary isn’t empty.

### Transforming a Dictionary’s Elements

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, that don’t contain elements satisfying the given predicate.

func reversed() -> [Self.Element]

Returns an array containing the elements of this sequence in reverse order.

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

