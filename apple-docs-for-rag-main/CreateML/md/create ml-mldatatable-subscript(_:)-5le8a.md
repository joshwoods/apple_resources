

- Create ML
- MLDataTable
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the table given a range expression of rows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(slice: R) -> MLDataTable where R : RangeExpression, R.Bound == Int { get }
```

## Parameters 

`slice`  

An interger range expression indicating which rows to include in the new data table.

## Return Value

A new data table.

## See Also

### Selecting Rows

subscript(Range&lt;Int>) -> MLDataTable

Creates a subset of the table given a range of rows.

func prefix(Int) -> MLDataTable

Creates a subset of the table given a number of initial rows.

func suffix(Int) -> MLDataTable

Creates a subset of the table given a number of final rows.

func intersect&lt;T>(T..., of: String) -> MLDataTable

Creates a subset of the table by including the rows that contain any of the given values in the given column.

