

- TabularData
- DataFrame
- DataFrame.Slice
-  base 

Instance Property

# base

The underlying data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var base: DataFrame { get }
```

## See Also

### Inspecting a Slice

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the slice.

var columns: [AnyColumnSlice]

The entire slice as a collection of columns.

var rows: DataFrame.Rows

The entire slice as a collection of rows.

