

- Create ML
- MLDataTable
-  sort(columnNamed:byIncreasingOrder:) 

Instance Method

# sort(columnNamed:byIncreasingOrder:)

Creates a new data table by sorting the table by the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func sort(
    columnNamed: String,
    byIncreasingOrder: Bool = true
) -> MLDataTable
```

## Parameters 

`columnNamed`  

The name of the column to sort the rows of data table.

`byIncreasingOrder`  

Set this value to true to sort the table in ascending order.

## Return Value

A new data table.

