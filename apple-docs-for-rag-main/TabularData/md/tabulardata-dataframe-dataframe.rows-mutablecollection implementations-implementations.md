

- TabularData
- DataFrame
- DataFrame.Rows
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

func reverse()

Reverses the elements of the collection in place.

func swapAt(Self.Index, Self.Index)

Exchanges the values at the specified indices of the collection.

func withContiguousMutableStorageIfAvailable&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the collection’s contiguous storage.

### Subscripts

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

Deprecated

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript(Range&lt;Self.Index>) -> Self.SubSequenceDeprecated

subscript&lt;R>(R) -> Self.SubSequence

