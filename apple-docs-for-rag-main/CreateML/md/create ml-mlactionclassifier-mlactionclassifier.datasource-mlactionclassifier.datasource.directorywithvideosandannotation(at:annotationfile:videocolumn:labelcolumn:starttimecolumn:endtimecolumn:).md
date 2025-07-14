

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  MLActionClassifier.DataSource.directoryWithVideosAndAnnotation(at:annotationFile:videoColumn:labelColumn:startTimeColumn:endTimeColumn:) 

Case

# MLActionClassifier.DataSource.directoryWithVideosAndAnnotation(at:annotationFile:videoColumn:labelColumn:startTimeColumn:endTimeColumn:)

The location of a directory of video files, and the location of an action annotation file.

macOS 11.0+

``` source
case directoryWithVideosAndAnnotation(
    at: URL,
    annotationFile: URL,
    videoColumn: String,
    labelColumn: String,
    startTimeColumn: String? = nil,
    endTimeColumn: String? = nil
)
```

## Parameters 

`at`  

The location of a directory that contains video files.

`annotationFile`  

The location of a JSON or CSV file with object annotations for the images.

`videoColumn`  

The name of the column that contains the URLs to the video files.

`labelColumn`  

The name of the column that contains the labels of the action the person demonstrates in the video file.

`startTimeColumn`  

The name of the column that contains the action’s starting-time in the video file.

`endTimeColumn `  

The name of the column that contains the action’s ending-time in the video file.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

The location of a folder with subfolders each of which contain sample videos of an action.

case labeledFiles(at: URL)

The location of a folder that contains video files whose names you use to label corresponding actions.

case labeledVideoData(table: MLDataTable, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data table that contains the locations of the video files and the action annotations.

Deprecated

