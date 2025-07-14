

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  MLActionClassifier.DataSource.labeledVideoData(table:videoColumn:labelColumn:startTimeColumn:endTimeColumn:) Deprecated

Case

# MLActionClassifier.DataSource.labeledVideoData(table:videoColumn:labelColumn:startTimeColumn:endTimeColumn:)

A data table that contains the locations of the video files and the action annotations.

macOS 11.0–14.0Deprecated

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

A data table that contains the video file locations and the action annotations.

`videoColumn`  

The name of the column that contains the URLs to the video files.

`labelColumn`  

The name of the column that contains the labels of the action the person demonstrates in the video file.

`startTimeColumn`  

The name of the column that contains the action’s starting-time index in the video file.

`endTimeColumn `  

The name of the column that contains the action’s ending-time index in the video file.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

The location of a folder with subfolders each of which contain sample videos of an action.

case labeledFiles(at: URL)

The location of a folder that contains video files whose names you use to label corresponding actions.

case directoryWithVideosAndAnnotation(at: URL, annotationFile: URL, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

The location of a directory of video files, and the location of an action annotation file.

