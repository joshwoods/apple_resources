

- TabularData
- DataFrame
- DataFrame.Slice
-  sorted(on:\_:\_:order:) 

Instance Method

# sorted(on:\_:\_:order:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to three columns that you select by their column identifiers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnID0: ColumnID,
    _ columnID1: ColumnID,
    _ columnID2: ColumnID,
    order: Order = .ascending
) -> DataFrame where T0 : Comparable, T1 : Comparable, T2 : Comparable
```

## Parameters 

`columnID0`  

The identifier of a column.

`columnID1`  

The identifier of a second column.

`columnID2`  

The identifier of a third column.

`order`  

A sorting order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Creating a Data Frame by Sorting Multiple Columns

func sorted&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to two columns that you select by their column identifiers.

