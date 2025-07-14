

- Create ML
- MLActivityClassifier
-  MLActivityClassifier.DataSource 

Enumeration

# MLActivityClassifier.DataSource

A data source for an activity classifier.

macOS 10.15+

``` source
enum DataSource
```

## Topics

### Creating a data source

case labeledDirectories(at: URL)

An activity classifier data source that uses a directory of directories that contain sensor data files.

case directoryWithDataAndAnnotation(at: URL, annotationFileName: String, timeStampColumn: String, labelStartTimeColumn: String, labelEndTimeColumn: String)

An activity classifier data source that uses a directory that contains sensor data files and one annotation file.

### Generating data tables from a data source

func labeledSensorData(featureColumns: [String], labelColumn: String?, recordingFileColumn: String?) throws -> MLDataTable

Generates a data table from the contents of the data source.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, featureColumns: [String], labelColumn: String, recordingFileColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

### Gathering annotated features

func gatherAnnotatedFeatures(featureColumns: [String], labelColumn: String, recordingFileColumn: String?) throws -> DataFrame

Processes the data source and returns a data frame that contains features, labels and file names.

### Getting the data frame

case dataFrame(DataFrame)

An activity classifier data source that uses a data frame containing sensor features and labels.

## See Also

### Supporting types

struct ModelParameters

Model training parameters that direct the training process for an activity classifier model.

