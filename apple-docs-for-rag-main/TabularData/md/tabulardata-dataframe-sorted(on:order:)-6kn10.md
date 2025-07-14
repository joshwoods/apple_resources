

- TabularData
- DataFrame
-  sorted(on:order:) 

Instance Method

# sorted(on:order:)

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(
    on columnID: ColumnID,
    order: Order = .ascending
) -> DataFrame where T : Comparable
```

## Parameters 

`order`  

A sorting order.

## Discussion

Note

Elements with a value of `nil` are less than all non-`nil` values.

