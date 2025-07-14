

- TabularData
- DataFrame
-  shape 

Instance Property

# shape

The number of rows and columns in the data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var shape: (rows: Int, columns: Int) { get }
```

## Parameters 

`rows`  

The number of rows in the data frame.

`columns`  

The number of columns in the data frame.

## See Also

### Inspecting a Data Frame

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var columns: [AnyColumn]

The entire data frame as a collection of columns.

var rows: DataFrame.Rows

The entire data frame as a collection of rows.

struct Rows

A collection of rows in a data frame.

var base: DataFrame

The underlying data frame.

func containsColumn&lt;T>(String, T.Type) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

