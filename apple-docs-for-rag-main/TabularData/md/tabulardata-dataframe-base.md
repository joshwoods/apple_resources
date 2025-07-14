

- TabularData
- DataFrame
-  base 

Instance Property

# base

The underlying data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var base: DataFrame { get }
```

## Discussion

For a DataFrame instance, this property is equivalent to `self`.

## See Also

### Inspecting a Data Frame

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the data frame.

var columns: [AnyColumn]

The entire data frame as a collection of columns.

var rows: DataFrame.Rows

The entire data frame as a collection of rows.

struct Rows

A collection of rows in a data frame.

func containsColumn&lt;T>(String, T.Type) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

