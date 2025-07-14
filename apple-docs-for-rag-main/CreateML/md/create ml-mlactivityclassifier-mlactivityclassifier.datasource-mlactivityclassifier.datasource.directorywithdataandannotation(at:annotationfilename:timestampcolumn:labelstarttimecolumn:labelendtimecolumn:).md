

- Create ML
- MLActivityClassifier
- MLActivityClassifier.DataSource
-  MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:) 

Case

# MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:)

An activity classifier data source that uses a directory that contains sensor data files and one annotation file.

macOS 10.15+

``` source
case directoryWithDataAndAnnotation(
    at: URL,
    annotationFileName: String,
    timeStampColumn: String,
    labelStartTimeColumn: String,
    labelEndTimeColumn: String
)
```

## Parameters 

`at`  

The location URL of a directory in the file system that contains sensor data files and an activity annotation file.

`annotationFileName`  

The name of the activity annotation file.

`timeStampColumn`  

The name of the column that contains the timestamps for each sensor data sample.

`labelStartTimeColumn`  

The name of the column that contains the activity’s starting-time index in the data file.

`labelEndTimeColumn`  

The name of the column that contains the activity’s ending-time index in the data file.

## Discussion

Create a data source by gathering all activity data files, and one annotation file, into a directory. Pass that directory’s URL and the relevant column names of the annotation file to MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

## See Also

### Creating a data source

case labeledDirectories(at: URL)

An activity classifier data source that uses a directory of directories that contain sensor data files.

