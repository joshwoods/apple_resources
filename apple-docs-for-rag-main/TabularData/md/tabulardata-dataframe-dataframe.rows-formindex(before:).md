

- TabularData
- DataFrame
- DataFrame.Rows
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

The index of the initial row in the collection.

var endIndex: Int

The index of the final row in the collection.

func index(before: Int) -> Int

Returns the row index immediately before a row index.

func index(after: Int) -> Int

Returns the row index immediately after a row index.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

