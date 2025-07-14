

- TabularData
- AnyColumnSlice
-  index(after:) 

Instance Method

# index(after:)

Returns the index immediately after an element index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func index(after i: Int) -> Int
```

## Parameters 

`i`  

A valid index to an element in the column slice.

## See Also

### Retrieving an Index

var startIndex: Int

The index of the initial element in the column slice.

var endIndex: Int

The index of the final element in the column slice.

func index(before: Int) -> Int

Returns the index immediately before an element index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

