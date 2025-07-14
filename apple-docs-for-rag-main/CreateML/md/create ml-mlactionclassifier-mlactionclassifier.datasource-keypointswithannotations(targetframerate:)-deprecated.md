

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  keypointsWithAnnotations(targetFrameRate:) Deprecated

Instance Method

# keypointsWithAnnotations(targetFrameRate:)

Generates a data table with action annotations of the data source.

macOS 11.0–14.0Deprecated

``` source
func keypointsWithAnnotations(targetFrameRate: Double = MLActionClassifier.__Defaults.targetFrameRate) throws -> MLDataTable
```

Deprecated

Use extractKeypoints(targetFrameRate:)

## Parameters 

`targetFrameRate`  

The number of frames per second the method uses to extract body landmarks from the data source. This no effect if the data source is an MLActionClassifier.DataSource.labeledKeypointsDataFrame(_:sessionIdColumn:labelColumn:featureColumn:) or an MLActionClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:).

## Return Value

A data table.

## See Also

### Generating data tables from a data source

func videosWithAnnotations() throws -> MLDataTable

Generates a data table of the data source’s video URL locations and action annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

