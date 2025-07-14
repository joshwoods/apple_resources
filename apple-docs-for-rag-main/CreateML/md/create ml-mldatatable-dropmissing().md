

- Create ML
- MLDataTable
-  dropMissing() 

Instance Method

# dropMissing()

Creates a subset of the table by removing any row missing one or more values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func dropMissing() -> MLDataTable
```

## Return Value

A new data table.

## See Also

### Discarding Rows

func dropDuplicates() -> MLDataTable

Creates a subset of the table by removing all duplicate rows.

func exclude&lt;T>(T..., of: String) -> MLDataTable

Creates a subset of the table by excluding the rows that contain any of the given values in the given column.

func randomSample(by: Double, seed: Int) -> MLDataTable

Creates a subset of the table by randomly selecting the given proportion of rows.

