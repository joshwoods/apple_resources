

- Create ML
- MLActivityClassifier
-  evaluation(on:featureColumns:labelColumn:recordingFileColumn:) Deprecated

Instance Method

# evaluation(on:featureColumns:labelColumn:recordingFileColumn:)

Generates metrics describing the activity classifier’s performance on labeled activities in a data table.

macOS 10.15–14.0Deprecated

``` source
func evaluation(
    on testingData: MLDataTable,
    featureColumns: [String],
    labelColumn: String,
    recordingFileColumn: String
) -> MLClassifierMetrics
```

## Parameters 

`testingData`  

The activity data that you provide to test this model, contained in an MLDataTable.

`featureColumns`  

The names of the columns that contain the sensor data.

`labelColumn`  

The name of the column that contain the activity labels.

`recordingFileColumn`  

The name of the column that contain the recording file names.

## Return Value

An MLClassifierMetrics instance.

## See Also

### Evaluating an activity classifier

func evaluation(on: MLActivityClassifier.DataSource, featureColumns: [String], labelColumn: String?, recordingFileColumn: String?) -> MLClassifierMetrics

Generates metrics describing the activity classifier’s performance on labeled activities in a data source.

