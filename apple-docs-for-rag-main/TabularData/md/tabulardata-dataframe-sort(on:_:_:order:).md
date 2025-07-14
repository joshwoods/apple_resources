

- TabularData
- DataFrame
-  sort(on:\_:\_:order:) 

Instance Method

# sort(on:\_:\_:order:)

Arranges the rows of a data frame according to three columns that you select by their column identifiers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func sort(
    on columnID0: ColumnID,
    _ columnID1: ColumnID,
    _ columnID2: ColumnID,
    order: Order = .ascending
) where T0 : Comparable, T1 : Comparable, T2 : Comparable
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

### Sorting a Data Frame

func sort(on: String, order: Order)

Arranges the rows of a data frame according to a column that you select by its name.

func sort&lt;T>(on: String, T.Type, order: Order)

Arranges the rows of a data frame according to a column that you select by its name and type.

func sort&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its name and type, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its column identifier, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, order: Order)

Arranges the rows of a data frame according to a column that you select by its column identifier.

func sort&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order)

Arranges the rows of a data frame according to two columns that you select by their column identifiers.

