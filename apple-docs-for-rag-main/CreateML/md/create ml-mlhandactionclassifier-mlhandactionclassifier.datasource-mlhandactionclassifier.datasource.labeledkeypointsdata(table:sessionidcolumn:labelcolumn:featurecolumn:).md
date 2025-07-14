

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  MLHandActionClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:) 

Case

# MLHandActionClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:)

Creates a data source from a data table of hand action observations that each contain the locations of each hand joint and an annotation.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
case labeledKeypointsData(
    table: MLDataTable,
    sessionIdColumn: String = __Defaults.sessionIdColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    featureColumn: String = __Defaults.featureColumnName
)
```

## Parameters 

`table `  

A data table that contains the hand-joint locations and annotations for a set of hand actions.

`sessionIdColumn`  

The name of the column in the data table that contains the session identifiers.

`labelColumn`  

The name of the column in the data table that contains the hand action label names.

`featureColumn`  

The name of the column in the data table that contains the hand-joint location data. Each entry in the column must be an MLMultiArray instance — which you must wrap in an MLDataValue.MultiArrayType — that contains three dimensions:

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

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data frame of hand action observations that each contain the locations of each hand joint and an annotation.

