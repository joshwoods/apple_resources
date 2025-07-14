

- Create ML
- MLActivityClassifier
- MLActivityClassifier.DataSource
-  labeledSensorData(featureColumns:labelColumn:recordingFileColumn:) Deprecated

Instance Method

# labeledSensorData(featureColumns:labelColumn:recordingFileColumn:)

Generates a data table from the contents of the data source.

macOS 10.15–14.0Deprecated

``` source
func labeledSensorData(
    featureColumns: [String],
    labelColumn: String? = nil,
    recordingFileColumn: String? = nil
) throws -> MLDataTable
```

Deprecated

Use gatherAnnotatedFeatures(featureColumns:labelColumn:recordingFileColumn:)

## Parameters 

`featureColumns`  

The names of the feature columns the method includes in the MLDataTable it generates.

`labelColumn`  

The name of the label column. This parameter must not be `nil` if the data source uses MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

`recordingFileColumn`  

The name of the column with the recording file names. This parameter must not be `nil` if the data source uses MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

## Return Value

A new MLDataTable instance.

## Discussion

The `labelColumn` and `recordingFileColumn` parameters are optional if the data source is MLActivityClassifier.DataSource.labeledDirectories(at:). If `nil`, the method names the data table’s label column and data file column “label” and “recordingFile”, respectively.

## See Also

### Generating data tables from a data source

func stratifiedSplit(proportions: [Double], seed: Int, featureColumns: [String], labelColumn: String, recordingFileColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

