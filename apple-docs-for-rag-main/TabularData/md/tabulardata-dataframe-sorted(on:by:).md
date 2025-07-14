

- TabularData
- DataFrame
-  sorted(on:by:) 

Instance Method

# sorted(on:by:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier, with a predicate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnID: ColumnID,
    by areInIncreasingOrder: (T, T) throws -> Bool
) rethrows -> DataFrame
```

## Parameters 

`columnID`  

The identifier of a column.

`areInIncreasingOrder`  

A closure that returns a Boolean that indicates whether the two elements are in increasing order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Sorting a Column

func sorted&lt;T>(on: String, T.Type, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type.

func sorted&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type, with a predicate.

