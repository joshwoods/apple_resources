

- TabularData
- DiscontiguousColumnSlice
-  startIndex 

Instance Property

# startIndex

The index of the initial element in the column slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var startIndex: Int { get }
```

## See Also

### Retrieving an Index

var endIndex: Int

The index of the final element in the column slice.

func index(before: Int) -> Int

Returns the index immediately before an element index.

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(Self.Index, offsetBy: Int) -> Self.Index

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

