

- TabularData
- DataFrame
-  sort(on:order:) 

Instance Method

# sort(on:order:)

Arranges the rows of a data frame according to a column that you select by its column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func sort(
    on columnID: ColumnID,
    order: Order = .ascending
) where T : Comparable
```

## Parameters 

`order`  

A sorting order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

## See Also

### Sorting a Data Frame

func sort(on: String, order: Order)

Arranges the rows of a data frame according to a column that you select by its name.

func sort&lt;T>(on: String, T.Type, order: Order)

Arranges the rows of a data frame according to a column that you select by its name and type.

func sort&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its name and type, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its column identifier, with a predicate.

func sort&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order)

Arranges the rows of a data frame according to two columns that you select by their column identifiers.

func sort&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, order: Order)

Arranges the rows of a data frame according to three columns that you select by their column identifiers.

