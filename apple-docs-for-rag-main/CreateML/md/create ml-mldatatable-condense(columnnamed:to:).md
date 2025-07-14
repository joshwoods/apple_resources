

- Create ML
- MLDataTable
-  condense(columnNamed:to:) 

Instance Method

# condense(columnNamed:to:)

Creates a new data table where duplicate row values in the given column are condensed into a new sequence-type column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func condense(
    columnNamed: String,
    to: String
) -> MLDataTable
```

## Parameters 

`columnNamed`  

The name of the column to condense.

`to`  

The name of the new condensed column.

## Return Value

A new data table.

## Discussion

This function performs the inverse of expand(columnNamed:to:).

