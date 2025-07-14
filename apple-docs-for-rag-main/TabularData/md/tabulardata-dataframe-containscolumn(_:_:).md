

- TabularData
- DataFrame
-  containsColumn(\_:\_:) 

Instance Method

# containsColumn(\_:\_:)

Returns a Boolean value indicating whether the data frame contains a column.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
func containsColumn(
    _ name: String,
    _ type: T.Type
) -> Bool
```

## Parameters 

`name`  

A column name.

`type`  

An element type.

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

var base: DataFrame

The underlying data frame.

