

- Swift
- Swift Standard Library
- Collections
- CollectionOfOne
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: CollectionOfOne&lt;Element>.Index

The “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: CollectionOfOne&lt;Element>.Index

The position of the first element.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: CollectionOfOne&lt;Element>.Index) -> CollectionOfOne&lt;Element>.Index

Returns the position immediately after the given index.

func index(before: CollectionOfOne&lt;Element>.Index) -> CollectionOfOne&lt;Element>.Index

Returns the position immediately before the given index.

### Subscripts

subscript(Range&lt;Int>) -> CollectionOfOne&lt;Element>.SubSequence

Accesses a contiguous subrange of the collection’s elements.

subscript(Int) -> Element

Accesses the element at the specified position.

