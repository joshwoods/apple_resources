

- Create ML
- MLActionClassifier
-  MLActionClassifier.DataSource 

Enumeration

# MLActionClassifier.DataSource

A data source for an action classifier.

macOS 11.0+

``` source
enum DataSource
```

## Mentioned in 

Building an Action Classifier Data Source

## Topics

### Creating a data source

case labeledDirectories(at: URL)

The location of a folder with subfolders each of which contain sample videos of an action.

case labeledFiles(at: URL)

The location of a folder that contains video files whose names you use to label corresponding actions.

case directoryWithVideosAndAnnotation(at: URL, annotationFile: URL, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

The location of a directory of video files, and the location of an action annotation file.

case labeledVideoData(table: MLDataTable, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data table that contains the locations of the video files and the action annotations.

Deprecated

### Extracting key points

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

A data source made up of keypoints in a data frame.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

A data table that contains the human body landmark movement data.

Deprecated

case labeledVideoDataFrame(DataFrame, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data source made up of video references in a data frame.

### Getting annotated file names

func gatherAnnotatedFileNames() throws -> DataFrame?

Processes the data source and returns a data frame that contains file URLs and annotations.

### Generating data tables from a data source

func videosWithAnnotations() throws -> MLDataTable

Generates a data table of the data source’s video URL locations and action annotations.

Deprecated

func keypointsWithAnnotations(targetFrameRate: Double) throws -> MLDataTable

Generates a data table with action annotations of the data source.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

## See Also

### Supporting types

struct ModelParameters

Parameters that affect the training process of an action classifier.

