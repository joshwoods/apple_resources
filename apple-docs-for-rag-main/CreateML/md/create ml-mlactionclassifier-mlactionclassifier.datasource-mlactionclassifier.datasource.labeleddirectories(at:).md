

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  MLActionClassifier.DataSource.labeledDirectories(at:) 

Case

# MLActionClassifier.DataSource.labeledDirectories(at:)

The location of a folder with subfolders each of which contain sample videos of an action.

macOS 11.0+

``` source
case labeledDirectories(at: URL)
```

## Discussion

The action classifier task uses each subfolder’s name as the label for an action.

## See Also

### Creating a data source

case labeledFiles(at: URL)

The location of a folder that contains video files whose names you use to label corresponding actions.

case directoryWithVideosAndAnnotation(at: URL, annotationFile: URL, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

The location of a directory of video files, and the location of an action annotation file.

case labeledVideoData(table: MLDataTable, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data table that contains the locations of the video files and the action annotations.

Deprecated

