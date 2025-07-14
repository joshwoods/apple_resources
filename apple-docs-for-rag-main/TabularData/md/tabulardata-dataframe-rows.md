

- TabularData
- DataFrame
-  rows 

Instance Property

# rows

The entire data frame as a collection of rows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var rows: DataFrame.Rows { get set }
```

## See Also

### Inspecting a Data Frame

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the data frame.

var columns: [AnyColumn]

The entire data frame as a collection of columns.

struct Rows

A collection of rows in a data frame.

var base: DataFrame

The underlying data frame.

func containsColumn&lt;T>(String, T.Type) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

