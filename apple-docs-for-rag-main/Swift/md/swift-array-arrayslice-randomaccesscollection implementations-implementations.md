

- Swift
- Array
- ArraySlice
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: Int

The array’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: Int

The position of the first element in a nonempty array.

### Instance Methods

func distance(from: Int, to: Int) -> Int

Returns the distance between two indices.

func formIndex(after: inout Int)

Replaces the given index with its successor.

func formIndex(before: inout Int)

Replaces the given index with its predecessor.

func index(Int, offsetBy: Int) -> Int

Returns an index that is the specified distance from the given index.

func index(Int, offsetBy: Int, limitedBy: Int) -> Int?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: Int) -> Int

Returns the position immediately after the given index.

func index(before: Int) -> Int

Returns the position immediately before the given index.

### Subscripts

subscript(Int) -> Element

Accesses the element at the specified position.

subscript(Range&lt;Int>) -> ArraySlice&lt;Element>

Accesses a contiguous subrange of the array’s elements.

### Type Aliases

typealias Index

The index type for arrays, `Int`.

typealias Indices

The type that represents the indices that are valid for subscripting an array, in ascending order.

