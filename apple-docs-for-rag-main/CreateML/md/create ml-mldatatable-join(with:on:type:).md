

- Create ML
- MLDataTable
-  join(with:on:type:) 

Instance Method

# join(with:on:type:)

Creates a new data table by merging two data tables by the given columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func join(
    with: MLDataTable,
    on columnsNamed: String...,
    type: MLDataTable.JoinType = .inner
) -> MLDataTable
```

## Parameters 

`with`  

Another data table to merge with this data table.

`columnsNamed`  

The name of the columns to perform the `join` operation on. The method merges all rows with matching values in these columns.

If you do not provide any column names, the method uses all the columns present in both tables.

`type`  

The type of `join` operation, which are equivalent to SQL `join` types.

## Return Value

A new data table.

## See Also

### Merging Data Tables

enum JoinType

Join types available for MLDataTable join operations.

