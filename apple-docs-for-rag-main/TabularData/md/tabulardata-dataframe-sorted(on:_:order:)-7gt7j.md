

- TabularData
- DataFrame
-  sorted(on:\_:order:) 

Instance Method

# sorted(on:\_:order:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnName: String,
    _ type: T.Type,
    order: Order = .ascending
) -> DataFrame where T : Comparable
```

## Parameters 

`columnName`  

The name of a column.

`type`  

The column’s type.

`order`  

A sorting order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Sorting a Column

func sorted&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type, with a predicate.

func sorted&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier, with a predicate.

