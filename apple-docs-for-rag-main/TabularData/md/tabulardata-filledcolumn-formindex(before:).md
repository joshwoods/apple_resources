

- TabularData
- FilledColumn
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

var startIndex: Base.Index

The index of the initial element in the column.

var endIndex: Base.Index

The index of the final element in the column.

func index(before: Base.Index) -> Base.Index

Returns the row index immediately before a row index.

func index(after: Base.Index) -> Base.Index

Returns the position immediately after an index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

