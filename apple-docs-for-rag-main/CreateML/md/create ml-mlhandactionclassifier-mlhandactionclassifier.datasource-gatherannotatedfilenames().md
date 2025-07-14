

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  gatherAnnotatedFileNames() 

Instance Method

# gatherAnnotatedFileNames()

Processes the data source and returns a data frame that contains file URLs and annotations.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func gatherAnnotatedFileNames() throws -> DataFrame?
```

## Discussion

This method collects file names from the filesystem if necessary. If the data source is already in table format it renames the columns to the default column names. This method returns nil if the data source contains key points.

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

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

