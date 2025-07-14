

- Create ML
- MLDataTable
-  exclude(\_:of:) 

Instance Method

# exclude(\_:of:)

Creates a subset of the table by excluding the rows that contain any of the given values in the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func exclude(
    _ values: T...,
    of columnNamed: String
) -> MLDataTable where T : MLDataValueConvertible
```

## Parameters 

`values`  

The values to exclude from the new table.

`columnNamed`  

The name of the column to search for excluded values.

## Return Value

A new data table.

## See Also

### Discarding Rows

func dropMissing() -> MLDataTable

Creates a subset of the table by removing any row missing one or more values.

func dropDuplicates() -> MLDataTable

Creates a subset of the table by removing all duplicate rows.

func randomSample(by: Double, seed: Int) -> MLDataTable

Creates a subset of the table by randomly selecting the given proportion of rows.

