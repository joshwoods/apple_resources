

- MusicKit
- MusicItemCollection
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var indices: MusicItemCollection&lt;MusicItemType>.Indices

The indices that are valid for subscripting the collection, in ascending order.

### Instance Methods

func distance(from: MusicItemCollection&lt;MusicItemType>.Index, to: MusicItemCollection&lt;MusicItemType>.Index) -> Int

Returns the distance between two indices.

func formIndex(after: inout MusicItemCollection&lt;MusicItemType>.Index)

Replaces the given index with its successor.

func formIndex(before: inout MusicItemCollection&lt;MusicItemType>.Index)

Replaces the given index with its predecessor.

func index(MusicItemCollection&lt;MusicItemType>.Index, offsetBy: Int) -> MusicItemCollection&lt;MusicItemType>.Index

Returns an index that is the specified distance from the given index.

func index(MusicItemCollection&lt;MusicItemType>.Index, offsetBy: Int, limitedBy: MusicItemCollection&lt;MusicItemType>.Index) -> MusicItemCollection&lt;MusicItemType>.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: MusicItemCollection&lt;MusicItemType>.Index) -> MusicItemCollection&lt;MusicItemType>.Index

Returns the position immediately after the given index.

func index(before: MusicItemCollection&lt;MusicItemType>.Index) -> MusicItemCollection&lt;MusicItemType>.Index

Returns the position immediately before the given index.

### Subscripts

subscript(Range&lt;MusicItemCollection&lt;MusicItemType>.Index>) -> MusicItemCollection&lt;MusicItemType>.SubSequence

Accesses a contiguous subrange of the collection’s elements.

