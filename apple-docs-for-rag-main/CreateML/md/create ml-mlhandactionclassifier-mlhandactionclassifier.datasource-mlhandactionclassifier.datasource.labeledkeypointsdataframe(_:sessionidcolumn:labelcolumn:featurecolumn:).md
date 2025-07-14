

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  MLHandActionClassifier.DataSource.labeledKeypointsDataFrame(\_:sessionIdColumn:labelColumn:featureColumn:) 

Case

# MLHandActionClassifier.DataSource.labeledKeypointsDataFrame(\_:sessionIdColumn:labelColumn:featureColumn:)

Creates a data source from a data frame of hand action observations that each contain the locations of each hand joint and an annotation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case labeledKeypointsDataFrame(
    DataFrame,
    sessionIdColumn: String = __Defaults.sessionIdColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    featureColumn: String = __Defaults.featureColumnName
)
```

## Parameters 

`dataFrame `  

A data frame that contains the hand-joint locations and annotations for a set of hand actions.

`sessionIdColumn`  

The name of the column in the data frame that contains the session identifiers.

`labelColumn`  

The name of the column in the data frame that contains the hand action label names.

`featureColumn`  

The name of the column in the data frame that contains the hand-joint location data. Each entry in the column must be a ShapedData instance that contains three dimensions:

- The first dimension has a size of one.

- The second dimension has three channels: the x-coordinate, the y-coordinate, and the confidence value, respectively.

- The third dimension has 21 channels, one for each hand joint.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain videos of a hand action.

case labeledFiles(at: URL)

Creates a data source from a folder that contains videos, each named after the hand action they represent.

case directoryWithVideosAndAnnotation(at: URL, annotationFile: URL, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

Creates a data source from a folder that contains videos and an annotation file.

case labeledVideoDataFrame(DataFrame, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

Creates a data source from a data frame that contains the location and annotation for a set of video files.

case labeledVideoData(table: MLDataTable, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

Creates a data source from a data table that contains the location and annotation for a set of video files.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand action observations that each contain the locations of each hand joint and an annotation.

