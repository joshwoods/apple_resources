

- TabularData
- DataFrame
- DataFrame.Slice
-  sorted(on:order:) 

Instance Method

# sorted(on:order:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnName: String,
    order: Order = .ascending
) -> DataFrame
```

## Parameters 

`columnName`  

The name of a column.

`order`  

A sorting order.

## Discussion

This is a convenience method that only works for columns of the following types:

- Bool

- Int

- Float

- Double

- Date

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Creating a Data Frame by Sorting a Column

func sorted&lt;T>(on: String, T.Type, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type.

func sorted&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type, with a predicate.

func sorted&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier, with a predicate.

