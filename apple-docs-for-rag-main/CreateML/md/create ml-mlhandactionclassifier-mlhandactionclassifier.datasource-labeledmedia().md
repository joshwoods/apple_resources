

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  labeledMedia() 

Instance Method

# labeledMedia()

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s video files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func labeledMedia() throws -> [String : [URL]]
```

## See Also

### Exporting a data source

func videosWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s video file URLs and a column of annotations.

Deprecated

func keypointsWithAnnotations(targetFrameRate: Double) throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and a column of hand action annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

func gatherAnnotatedFileNames() throws -> DataFrame?

Processes the data source and returns a data frame that contains file URLs and annotations.

