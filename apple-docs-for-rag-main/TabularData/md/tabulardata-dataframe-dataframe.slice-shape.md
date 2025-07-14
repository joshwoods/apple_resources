

- TabularData
- DataFrame
- DataFrame.Slice
-  shape 

Instance Property

# shape

The number of rows and columns in the slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var shape: (rows: Int, columns: Int) { get }
```

## Parameters 

`rows`  

The number of rows in the slice.

`columns`  

The number of columns in the slice.

## See Also

### Inspecting a Slice

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var columns: [AnyColumnSlice]

The entire slice as a collection of columns.

var rows: DataFrame.Rows

The entire slice as a collection of rows.

var base: DataFrame

The underlying data frame.

