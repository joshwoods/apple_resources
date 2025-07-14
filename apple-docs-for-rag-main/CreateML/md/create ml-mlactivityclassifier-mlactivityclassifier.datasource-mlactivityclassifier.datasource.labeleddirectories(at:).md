

- Create ML
- MLActivityClassifier
- MLActivityClassifier.DataSource
-  MLActivityClassifier.DataSource.labeledDirectories(at:) 

Case

# MLActivityClassifier.DataSource.labeledDirectories(at:)

An activity classifier data source that uses a directory of directories that contain sensor data files.

macOS 10.15+

``` source
case labeledDirectories(at: URL)
```

## Parameters 

`at`  

A URL of a directory in the file system that contains directories, each named with an activity label for the sensor data files.

## Discussion

Create a data source by organizing each activity’s data files into a directory and naming each directory with the label for that activity.

Note

Each data file must contain exactly one entire recording of an activity.

For example, to organize data files for an activity classifier that recognizes walking, jogging, and running, start by creating directories named “walk”, “jog”, and “run”. Place all the files of walking sensor data into the “walk” directory, and so on.

Next, gather all the activity directories into a directory and pass its URL to MLActivityClassifier.DataSource.labeledDirectories(at:).

## See Also

### Creating a data source

case directoryWithDataAndAnnotation(at: URL, annotationFileName: String, timeStampColumn: String, labelStartTimeColumn: String, labelEndTimeColumn: String)

An activity classifier data source that uses a directory that contains sensor data files and one annotation file.

