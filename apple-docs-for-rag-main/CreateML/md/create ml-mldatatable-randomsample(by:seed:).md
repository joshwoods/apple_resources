

- Create ML
- MLDataTable
-  randomSample(by:seed:) 

Instance Method

# randomSample(by:seed:)

Creates a subset of the table by randomly selecting the given proportion of rows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func randomSample(
    by proportion: Double,
    seed: Int = 42
) -> MLDataTable
```

## Parameters 

`proportion`  

The fraction of rows to sample from the original table. The value must be in the range `(0.0, 1.0)`.

`seed`  

A number that seeds a random number generator.

## Return Value

A new data table.

## See Also

### Discarding Rows

func dropMissing() -> MLDataTable

Creates a subset of the table by removing any row missing one or more values.

func dropDuplicates() -> MLDataTable

Creates a subset of the table by removing all duplicate rows.

func exclude&lt;T>(T..., of: String) -> MLDataTable

Creates a subset of the table by excluding the rows that contain any of the given values in the given column.

