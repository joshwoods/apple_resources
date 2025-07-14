

- Swift
- Swift Standard Library
- Collections
- ClosedRange
-  Collection Implementations 

API Collection

# Collection Implementations

## Topics

### Instance Properties

var endIndex: ClosedRange&lt;Bound>.Index

The range’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var isEmpty: Bool

A Boolean value indicating whether the range contains no elements.

var startIndex: ClosedRange&lt;Bound>.Index

The position of the first element in the range.

### Instance Methods

func distance(from: ClosedRange&lt;Bound>.Index, to: ClosedRange&lt;Bound>.Index) -> Int

Returns the distance between two indices.

func index(ClosedRange&lt;Bound>.Index, offsetBy: Int) -> ClosedRange&lt;Bound>.Index

Returns an index that is the specified distance from the given index.

func index(after: ClosedRange&lt;Bound>.Index) -> ClosedRange&lt;Bound>.Index

Returns the position immediately after the given index.

### Subscripts

subscript(ClosedRange&lt;Bound>.Index) -> Bound

Accesses the element at specified position.

subscript(Range&lt;ClosedRange&lt;Bound>.Index>) -> Slice&lt;ClosedRange&lt;Bound>>

Accesses a contiguous subrange of the collection’s elements.

### Type Aliases

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Enumerations

enum Index

A type that represents a position in the collection.

