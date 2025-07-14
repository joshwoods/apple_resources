

- TabularData
- DataFrame
-  sort(on:\_:order:) 

Instance Method

# sort(on:\_:order:)

Arranges the rows of a data frame according to a column that you select by its name and type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func sort(
    on columnName: String,
    _ type: T.Type,
    order: Order = .ascending
) where T : Comparable
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

### Sorting a Data Frame

func sort(on: String, order: Order)

Arranges the rows of a data frame according to a column that you select by its name.

func sort&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its name and type, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its column identifier, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, order: Order)

Arranges the rows of a data frame according to a column that you select by its column identifier.

func sort&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order)

Arranges the rows of a data frame according to two columns that you select by their column identifiers.

func sort&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, order: Order)

Arranges the rows of a data frame according to three columns that you select by their column identifiers.

