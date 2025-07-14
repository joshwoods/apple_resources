

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  keypointsWithAnnotations(targetFrameRate:) Deprecated

Instance Method

# keypointsWithAnnotations(targetFrameRate:)

Generates a data table that contains a column for hand joint locations and a column of hand action annotations.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
func keypointsWithAnnotations(targetFrameRate: Double = MLHandActionClassifier.__Defaults.targetFrameRate) throws -> MLDataTable
```

Deprecated

Use extractKeypoints(targetFrameRate:)

## Parameters 

`targetFrameRate`  

The number of frames per second the method uses to extract body landmarks from the data source.

This parameter has no effect if the data source is either:

- MLHandActionClassifier.DataSource.labeledKeypointsDataFrame(_:sessionIdColumn:labelColumn:featureColumn:)

- MLHandActionClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:)

## See Also

### Exporting a data source

func labeledMedia() throws -> [String : [URL]]

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s video files.

func videosWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s video file URLs and a column of annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

func gatherAnnotatedFileNames() throws -> DataFrame?

Processes the data source and returns a data frame that contains file URLs and annotations.

