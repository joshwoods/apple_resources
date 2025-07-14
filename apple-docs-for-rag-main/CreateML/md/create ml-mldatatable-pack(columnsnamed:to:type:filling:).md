

- Create ML
- MLDataTable
-  pack(columnsNamed:to:type:filling:) 

Instance Method

# pack(columnsNamed:to:type:filling:)

Creates a new data table with an additional column that contains the combined values of the given columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func pack(
    columnsNamed: String...,
    to: String,
    type: MLDataTable.PackType = .sequence,
    filling: MLDataValue = MLDataValue.invalid
) -> MLDataTable
```

## Parameters 

`columnsNamed`  

The name of the columns to compact.

`to`  

The name of the new condensed column.

`type`  

The collection type for the new column. Typically, the type is a sequence or a dictionary.

`filling`  

The value to fill in any missing values with.

## Return Value

A new data table.

## Discussion

This function performs the inverse of unpack(columnNamed:valueTypes:indexSubset:keySubset:).

## See Also

### Compacting Columns

enum PackType

The storage operations for combining multiple columns into one.

