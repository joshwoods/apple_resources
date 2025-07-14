

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.DataSource
-  MLHandActionClassifier.DataSource.labeledVideoData(table:videoColumn:labelColumn:startTimeColumn:endTimeColumn:) 

Case

# MLHandActionClassifier.DataSource.labeledVideoData(table:videoColumn:labelColumn:startTimeColumn:endTimeColumn:)

Creates a data source from a data table that contains the location and annotation for a set of video files.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
case labeledVideoData(
    table: MLDataTable,
    videoColumn: String = __Defaults.videoColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    startTimeColumn: String? = nil,
    endTimeColumn: String? = nil
)
```

## Parameters 

`table`  

A data table that contains the locations of annotations for each hand action video file.

`videoColumn`  

The name of the column in the data table that contains the video filenames.

`labelColumn`  

The name of the column in the data table that contains the hand action label names.

`startTimeColumn`  

The name of the column in the data table that contains the hand action’s starting-time index in the video file. Otherwise `nil`, if every video example starts at the beginning of the video file.

## Discussion

- endTimeColumn: The name of the column in the data table that contains the hand action’s ending-time in the video file. Otherwise `nil`, if every video example ends at the end of the video file.

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

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data frame of hand action observations that each contain the locations of each hand joint and an annotation.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand action observations that each contain the locations of each hand joint and an annotation.

