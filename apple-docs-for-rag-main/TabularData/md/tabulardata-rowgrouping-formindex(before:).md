

- TabularData
- RowGrouping
-  formIndex(before:) 

Instance Method

# formIndex(before:)

Replaces the given index with its predecessor.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formIndex(before i: inout Self.Index)
```

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

## See Also

### Retrieving an Index

var startIndex: Int

The index of the initial group in the row grouping.

var endIndex: Int

The index of the final group in the row grouping.

func index(before: Int) -> Int

Returns the index immediately before an element index.

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

