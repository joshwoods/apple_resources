

- Create ML
- MLDataTable
-  intersect(\_:of:) 

Instance Method

# intersect(\_:of:)

Creates a subset of the table by including the rows that contain any of the given values in the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func intersect(
    _ values: T...,
    of columnNamed: String
) -> MLDataTable where T : MLDataValueConvertible
```

## Parameters 

`values`  

The values to include from the new table.

`columnNamed`  

The name of the column to search for included values.

## Return Value

A new data table.

## See Also

### Selecting Rows

subscript(Range&lt;Int>) -> MLDataTable

Creates a subset of the table given a range of rows.

subscript&lt;R>(R) -> MLDataTable

Creates a subset of the table given a range expression of rows.

func prefix(Int) -> MLDataTable

Creates a subset of the table given a number of initial rows.

func suffix(Int) -> MLDataTable

Creates a subset of the table given a number of final rows.

