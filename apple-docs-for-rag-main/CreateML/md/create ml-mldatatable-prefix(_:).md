

- Create ML
- MLDataTable
-  prefix(\_:) 

Instance Method

# prefix(\_:)

Creates a subset of the table given a number of initial rows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func prefix(_ maxLength: Int = 10) -> MLDataTable
```

## Parameters 

`maxLength`  

The largest number of rows to use from the beginning of the data table. The default value is `10`.

## Return Value

A new data table.

## See Also

### Selecting Rows

subscript(Range&lt;Int>) -> MLDataTable

Creates a subset of the table given a range of rows.

subscript&lt;R>(R) -> MLDataTable

Creates a subset of the table given a range expression of rows.

func suffix(Int) -> MLDataTable

Creates a subset of the table given a number of final rows.

func intersect&lt;T>(T..., of: String) -> MLDataTable

Creates a subset of the table by including the rows that contain any of the given values in the given column.

