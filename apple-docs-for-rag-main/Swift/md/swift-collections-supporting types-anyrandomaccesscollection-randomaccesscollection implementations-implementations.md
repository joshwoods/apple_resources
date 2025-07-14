

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Collections
- Supporting Types
- AnyRandomAccessCollection
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: AnyRandomAccessCollection&lt;Element>.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: AnyRandomAccessCollection&lt;Element>.Index

The position of the first element in a non-empty collection.

### Instance Methods

func distance(from: AnyRandomAccessCollection&lt;Element>.Index, to: AnyRandomAccessCollection&lt;Element>.Index) -> Int

Returns the distance between two indices.

func formIndex(after: inout AnyRandomAccessCollection&lt;Element>.Index)

Replaces the given index with its successor.

func formIndex(before: inout AnyRandomAccessCollection&lt;Element>.Index)

Replaces the given index with its predecessor.

func index(AnyRandomAccessCollection&lt;Element>.Index, offsetBy: Int) -> AnyRandomAccessCollection&lt;Element>.Index

Returns an index that is the specified distance from the given index.

func index(AnyRandomAccessCollection&lt;Element>.Index, offsetBy: Int, limitedBy: AnyRandomAccessCollection&lt;Element>.Index) -> AnyRandomAccessCollection&lt;Element>.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: AnyRandomAccessCollection&lt;Element>.Index) -> AnyRandomAccessCollection&lt;Element>.Index

Returns the position immediately after the given index.

func index(before: AnyRandomAccessCollection&lt;Element>.Index) -> AnyRandomAccessCollection&lt;Element>.Index

Returns the position immediately before the given index.

### Subscripts

subscript(AnyRandomAccessCollection&lt;Element>.Index) -> Element

Accesses the element indicated by `position`.

subscript(Range&lt;AnyRandomAccessCollection&lt;Element>.Index>) -> AnyRandomAccessCollection&lt;Element>.SubSequence

Accesses a contiguous subrange of the collection’s elements.

