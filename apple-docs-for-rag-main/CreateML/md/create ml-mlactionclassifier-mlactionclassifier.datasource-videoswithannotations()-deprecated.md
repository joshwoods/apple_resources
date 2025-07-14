

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  videosWithAnnotations() Deprecated

Instance Method

# videosWithAnnotations()

Generates a data table of the data source’s video URL locations and action annotations.

macOS 11.0–14.0Deprecated

``` source
func videosWithAnnotations() throws -> MLDataTable
```

Deprecated

Use gatherAnnotatedFileNames()

## Return Value

A data table.

## Discussion

The data table includes a column for the annotation’s label, and if applicable, the annotation’s starting- and ending-time indices.

## See Also

### Generating data tables from a data source

func keypointsWithAnnotations(targetFrameRate: Double) throws -> MLDataTable

Generates a data table with action annotations of the data source.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

