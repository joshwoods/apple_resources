

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  stratifiedSplit(proportions:seed:labelColumn:) Deprecated

Instance Method

# stratifiedSplit(proportions:seed:labelColumn:)

Generates a data table by splitting the data source into strata.

macOS 11.0–14.0Deprecated

``` source
func stratifiedSplit(
    proportions: [Double],
    seed: Int = timestampSeed(),
    labelColumn: String
) throws -> MLDataTable
```

Deprecated

Use DataFrame.stratifiedSplit(on:by:)

## Parameters 

`proportions`  

An array of proportions, each in the range `[0.0, 1.0]`.

`seed`  

A seed number for the random-number generator.

`labelColumn`  

The name of the column that you want to stratify.

## Return Value

A new data table.

## See Also

### Generating data tables from a data source

func videosWithAnnotations() throws -> MLDataTable

Generates a data table of the data source’s video URL locations and action annotations.

Deprecated

func keypointsWithAnnotations(targetFrameRate: Double) throws -> MLDataTable

Generates a data table with action annotations of the data source.

Deprecated

