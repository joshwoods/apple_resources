

- Create ML
- MLDataTable
-  randomSplit(by:seed:) 

Instance Method

# randomSplit(by:seed:)

Creates two mutually exclusive, randomly divided subsets of the table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func randomSplit(
    by proportion: Double,
    seed: Int = 1
) -> (MLDataTable, MLDataTable)
```

## Return Value

Two new data tables.

## Mentioned in 

Creating a Text Classifier Model

## Discussion

- proportion: A value between `0.0` and `1.0` indicating the fraction of rows to go into one subset. The remaining rows go into the other subset.

  - seed: A random number generator seed. The default value is `1`.

