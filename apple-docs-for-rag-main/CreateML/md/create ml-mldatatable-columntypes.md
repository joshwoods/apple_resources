

- Create ML
- MLDataTable
-  columnTypes 

Instance Property

# columnTypes

The type of the data in each column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var columnTypes: [String : MLDataValue.ValueType] { get }
```

## Discussion

The keys in the dictionary provided by this column correspond to the names of the columns in the data table.

## See Also

### Getting information about a data table’s columns

var columnNames: MLDataTable.ColumnNames

The names of the columns in the data table.

struct ColumnNames

A collection of the names of the columns in a data table.

