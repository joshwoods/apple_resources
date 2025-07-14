

- TabularData
- DataFrame
-  columns 

Instance Property

# columns

The entire data frame as a collection of columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var columns: [AnyColumn] { get }
```

## See Also

### Inspecting a Data Frame

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the data frame.

var rows: DataFrame.Rows

The entire data frame as a collection of rows.

struct Rows

A collection of rows in a data frame.

var base: DataFrame

The underlying data frame.

func containsColumn&lt;T>(String, T.Type) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

