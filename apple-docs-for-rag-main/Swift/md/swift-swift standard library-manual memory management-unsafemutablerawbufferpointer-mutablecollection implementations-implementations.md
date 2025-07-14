

- Swift
- Swift Standard Library
- Manual Memory Management
- UnsafeMutableRawBufferPointer
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

func shuffle()

Shuffles the collection in place.

func shuffle&lt;T>(using: inout T)

Shuffles the collection in place, using the given generator as a source for randomness.

func sort()

Sorts the collection in place.

func sort(by: (Self.Element, Self.Element) throws -> Bool) rethrows

Sorts the collection in place, using the given predicate as the comparison between elements.

func swapAt(Int, Int)

Exchanges the byte values at the specified indices in this buffer’s memory.

func withContiguousMutableStorageIfAvailable&lt;R>((inout UnsafeMutableBufferPointer&lt;UnsafeMutableRawBufferPointer.Element>) throws -> R) rethrows -> R?

Executes a closure on the collection’s contiguous storage.

### Subscripts

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

Deprecated

subscript&lt;R>(R) -> Self.SubSequence

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript(Range&lt;Self.Index>) -> Self.SubSequenceDeprecated

subscript(Int) -> UnsafeMutableRawBufferPointer.Element

Accesses the byte at the given offset in the memory region as a `UInt8` value.

subscript(Range&lt;Int>) -> UnsafeMutableRawBufferPointer.SubSequence

Accesses the bytes in the specified memory region.

