

- Create ML Components
- ColumnSelection
-  ColumnSelection.numeric 

Case

# ColumnSelection.numeric

Select all numeric columns in the data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case numeric
```

## Discussion

Numeric columns are columns with elements of type `Int`, `UInt8`, `Float`, `Double`. Also arrays of those types and shaped arrays of those types.

## See Also

### Column selection types

case all

Select all columns in the data frame.

case exclude(columnNames: [String])

Selects all columns except the specified columns.

case include(columnNames: [String])

Selects only the specified columns.

