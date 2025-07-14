

- Swift
- Swift Standard Library
- Collections
- Range
-  Collection Implementations 

API Collection

# Collection Implementations

## Topics

### Instance Properties

var endIndex: Range&lt;Bound>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var indices: Range&lt;Bound>.Indices

The indices that are valid for subscripting the range, in ascending order.

var startIndex: Range&lt;Bound>.Index

The position of the first element in a nonempty collection.

### Instance Methods

func distance(from: Range&lt;Bound>.Index, to: Range&lt;Bound>.Index) -> Int

Returns the distance between two indices.

func index(Range&lt;Bound>.Index, offsetBy: Int) -> Range&lt;Bound>.Index

Returns an index that is the specified distance from the given index.

func index(after: Range&lt;Bound>.Index) -> Range&lt;Bound>.Index

Returns the position immediately after the given index.

### Subscripts

subscript(Range&lt;Range&lt;Bound>.Index>) -> Range&lt;Bound>

Accesses the subsequence bounded by the given range.

subscript(Range&lt;Bound>.Index) -> Range&lt;Bound>.Element

Accesses the element at specified position.

### Type Aliases

typealias Index

A type that represents a position in the range.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

