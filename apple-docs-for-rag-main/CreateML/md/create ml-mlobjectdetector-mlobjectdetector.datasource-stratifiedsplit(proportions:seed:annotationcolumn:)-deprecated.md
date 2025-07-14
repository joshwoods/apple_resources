

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  stratifiedSplit(proportions:seed:annotationColumn:) Deprecated

Instance Method

# stratifiedSplit(proportions:seed:annotationColumn:)

Generates a new data table by splitting the data source using the specified proportions.

macOS 10.15–14.0Deprecated

``` source
func stratifiedSplit(
    proportions: [Double],
    seed: Int = timestampSeed(),
    annotationColumn: String
) throws -> MLDataTable
```

Deprecated

Use DataFrame.stratifiedSplit(on:by:)

## Return Value

An MLDataTable containing the data source’s split contents.

## Discussion

- proportions: An array of doubles, each representing a portion of the data source. If these values don’t add up to `1.0`, the method normalizes the numbers so that they do.

- seed: The value the method uses to initialize the random-number generator, which affects how the method splits the data.

- annotationColumn: The name of the column the method uses to split the data.

