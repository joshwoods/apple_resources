

- TabularData
- DiscontiguousColumnSlice
-  index(\_:offsetBy:) 

Instance Method

# index(\_:offsetBy:)

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func index(
    _ i: Self.Index,
    offsetBy distance: Int
) -> Self.Index
```

## See Also

### Retrieving an Index

var startIndex: Int

The index of the initial element in the column slice.

var endIndex: Int

The index of the final element in the column slice.

func index(before: Int) -> Int

Returns the index immediately before an element index.

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

