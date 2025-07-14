

- TabularData
- DataFrame
- DataFrame.Slice
-  filter(on:\_:) 

Instance Method

# filter(on:\_:)

Returns a selection of rows that satisfy a predicate in the columns you select by column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func filter(
    on columnID: ColumnID,
    _ isIncluded: (T?) throws -> Bool
) rethrows -> DataFrame.Slice
```

## Parameters 

`columnID`  

The identifier of a column in the slice.

`isIncluded`  

A predicate closure that receives an element of the column as its argument, and returns a Boolean that indicates whether the slice includes the element’s row.

## Return Value

A data frame slice that contains the rows that satisfy the predicate.

## See Also

### Creating a Slice by Filtering Rows

func filter&lt;T>(on: String, T.Type, (T?) throws -> Bool) rethrows -> DataFrame.Slice

Returns a selection of rows that satisfy a predicate in the columns you select by name.

