

- Create ML
- MLDataTable
-  expand(columnNamed:to:) 

Instance Method

# expand(columnNamed:to:)

Creates a new data table where duplicate row values in the given column are condensed into a new sequence-type column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func expand(
    columnNamed: String,
    to: String
) -> MLDataTable
```

## Parameters 

`columnNamed`  

The name of the column to expand.

`to`  

The name of the new expanded column.

## Return Value

A new data table.

## Discussion

This function performs the inverse of condense(columnNamed:to:).

