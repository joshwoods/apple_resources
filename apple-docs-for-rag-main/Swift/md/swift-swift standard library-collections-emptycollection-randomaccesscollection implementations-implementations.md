

- Swift
- Swift Standard Library
- Collections
- EmptyCollection
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: EmptyCollection&lt;Element>.Index

Always zero, just like `startIndex`.

var startIndex: EmptyCollection&lt;Element>.Index

Always zero, just like `endIndex`.

### Instance Methods

func distance(from: EmptyCollection&lt;Element>.Index, to: EmptyCollection&lt;Element>.Index) -> Int

The distance between two indexes (always zero).

func index(EmptyCollection&lt;Element>.Index, offsetBy: Int) -> EmptyCollection&lt;Element>.Index

Returns an index that is the specified distance from the given index.

func index(EmptyCollection&lt;Element>.Index, offsetBy: Int, limitedBy: EmptyCollection&lt;Element>.Index) -> EmptyCollection&lt;Element>.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: EmptyCollection&lt;Element>.Index) -> EmptyCollection&lt;Element>.Index

Always traps.

func index(before: EmptyCollection&lt;Element>.Index) -> EmptyCollection&lt;Element>.Index

Always traps.

### Subscripts

subscript(EmptyCollection&lt;Element>.Index) -> Element

Accesses the element at the given position.

subscript(Range&lt;EmptyCollection&lt;Element>.Index>) -> EmptyCollection&lt;Element>.SubSequence

Accesses a contiguous subrange of the collection’s elements.

### Type Aliases

typealias Index

A type that represents a valid position in the collection.

