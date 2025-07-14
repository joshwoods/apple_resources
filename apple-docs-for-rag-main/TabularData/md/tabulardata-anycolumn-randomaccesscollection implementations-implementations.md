

- TabularData
- AnyColumn
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: Int

The index of the final element in the column.

var startIndex: Int

The index of the initial element in the column.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(before: Int) -> Int

Returns the index immediately before an element index.

### Subscripts

subscript(Range&lt;Int>) -> AnyColumnSlice

Accesses a contiguous subrange of the elements.

subscript(Int) -> Any?

Accesses an element at an index.

