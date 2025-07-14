

- Create ML
- MLDataTable
-  fillMissing(columnNamed:with:) 

Instance Method

# fillMissing(columnNamed:with:)

Creates a modified copy of the table by filling in the missing values in the named column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func fillMissing(
    columnNamed: String,
    with value: MLDataValue
) -> MLDataTable
```

## Parameters 

`columnNamed`  

The name of the column with missing values.

`value`  

An `MLDataValue` to put in place for every missing value in the column.

## Return Value

A new data table.

