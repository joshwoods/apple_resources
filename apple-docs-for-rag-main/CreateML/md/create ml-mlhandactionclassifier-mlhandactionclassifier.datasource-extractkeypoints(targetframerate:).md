

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  extractKeypoints(targetFrameRate:) 

Instance Method

# extractKeypoints(targetFrameRate:)

Extracts key points from video files if necessary.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func extractKeypoints(targetFrameRate: Double = MLHandActionClassifier.__Defaults.targetFrameRate) throws -> DataFrame
```

## Parameters 

`targetFrameRate`  

The number of frames per second the method uses to extract body landmarks from the data source.

## Return Value

A data frame that contains a column for hand joint locations and a column of hand action annotations.

## Discussion

If the data source already contains keypoints, this method just renames the data frame columns to the defaults.

## See Also

### Exporting a data source

func labeledMedia() throws -> [String : [URL]]

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s video files.

func videosWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s video file URLs and a column of annotations.

Deprecated

func keypointsWithAnnotations(targetFrameRate: Double) throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and a column of hand action annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

func gatherAnnotatedFileNames() throws -> DataFrame?

Processes the data source and returns a data frame that contains file URLs and annotations.

