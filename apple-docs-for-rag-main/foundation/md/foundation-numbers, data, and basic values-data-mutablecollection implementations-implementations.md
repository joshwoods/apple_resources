

- Foundation
- Numbers, Data, and Basic Values
- Data
-  MutableCollection Implementations 

API Collection

# MutableCollection Implementations

## Topics

### Instance Methods

func moveSubranges(RangeSet&lt;Self.Index>, to: Self.Index) -> Range&lt;Self.Index>

Moves the elements in the given subranges to just before the element at the specified index.

func partition(by: (Self.Element) throws -> Bool) rethrows -> Self.Index

Reorders the elements of the collection such that all the elements that match the given predicate are after all the elements that don’t match.

func partition(by: (Self.Element) throws -> Bool) rethrows -> Self.Index

Reorders the elements of the collection such that all the elements that match the given predicate are after all the elements that don’t match.

func removeSubranges(RangeSet&lt;Self.Index>)

Removes the elements at the given indices.

func reverse()

Reverses the elements of the collection in place.

func shuffle()

Shuffles the collection in place.

func shuffle&lt;T>(using: inout T)

Shuffles the collection in place, using the given generator as a source for randomness.

func sort()

Sorts the collection in place.

func sort(by: (Self.Element, Self.Element) throws -> Bool) rethrows

Sorts the collection in place, using the given predicate as the comparison between elements.

func sort&lt;S, Comparator>(using: S)

Sorts the collection using the given array of `SortComparator`s to compare elements.

func sort&lt;Comparator>(using: Comparator)

Sorts the collection using the given comparator to compare elements.

func swapAt(Self.Index, Self.Index)

Exchanges the values at the specified indices of the collection.

func withContiguousMutableStorageIfAvailable&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the collection’s contiguous storage.

### Subscripts

subscript&lt;R>(R) -> Self.SubSequence

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

Deprecated

subscript(Range&lt;Self.Index>) -> Self.SubSequenceDeprecated

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

