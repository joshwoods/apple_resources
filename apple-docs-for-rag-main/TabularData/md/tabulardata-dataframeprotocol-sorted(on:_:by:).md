

- TabularData
- DataFrameProtocol
-  sorted(on:\_:by:) 

Instance Method

# sorted(on:\_:by:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type, with a predicate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnName: String,
    _ type: T.Type,
    by areInIncreasingOrder: (T, T) throws -> Bool
) rethrows -> DataFrame
```

## Parameters 

`columnName`  

The name of a column.

`type`  

The column’s type.

`areInIncreasingOrder`  

A closure that returns a Boolean that indicates whether the two elements are in increasing order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Creating a Data Frame by Sorting a Column

func sorted(on: String, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name.

func sorted&lt;T>(on: String, T.Type, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type.

func sorted&lt;T>(on: ColumnID&lt;T>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier.

func sorted&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier, with a predicate.

