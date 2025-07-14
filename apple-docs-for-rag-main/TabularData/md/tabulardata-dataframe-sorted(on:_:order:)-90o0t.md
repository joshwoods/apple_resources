

- TabularData
- DataFrame
-  sorted(on:\_:order:) 

Instance Method

# sorted(on:\_:order:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to two columns that you select by their column identifiers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnID0: ColumnID,
    _ columnID1: ColumnID,
    order: Order = .ascending
) -> DataFrame where T0 : Comparable, T1 : Comparable
```

## Parameters 

`columnID0`  

The identifier of a column.

`columnID1`  

The identifier of another column.

`order`  

A sorting order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Sorting Multiple Columns

func sorted&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to three columns that you select by their column identifiers.

