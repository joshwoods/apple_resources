

- TabularData
- DataFrame
- DataFrame.Slice
-  rows 

Instance Property

# rows

The entire slice as a collection of rows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var rows: DataFrame.Rows { get set }
```

## See Also

### Inspecting a Slice

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the slice.

var columns: [AnyColumnSlice]

The entire slice as a collection of columns.

var base: DataFrame

The underlying data frame.

