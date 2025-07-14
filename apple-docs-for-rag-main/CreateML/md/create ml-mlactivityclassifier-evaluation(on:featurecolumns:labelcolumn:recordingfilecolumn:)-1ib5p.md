

- Create ML
- MLActivityClassifier
-  evaluation(on:featureColumns:labelColumn:recordingFileColumn:) 

Instance Method

# evaluation(on:featureColumns:labelColumn:recordingFileColumn:)

Generates metrics describing the activity classifier’s performance on labeled activities in a data source.

macOS 10.15+

``` source
func evaluation(
    on testingData: MLActivityClassifier.DataSource,
    featureColumns: [String],
    labelColumn: String? = nil,
    recordingFileColumn: String? = nil
) -> MLClassifierMetrics
```

## Parameters 

`testingData`  

The activity data that you provide to test this model, contained in an MLActivityClassifier.DataSource.

`featureColumns`  

The names of the columns that contain sensor data.

`labelColumn`  

The name of the column that contain the activity labels. The method ignores this parameter if the data source uses a labeled directory.

`recordingFileColumn`  

The name of the column that contain the recording file names. The method ignores this parameter if the data source uses a labeled directory.

## Return Value

An MLClassifierMetrics instance.

## See Also

### Evaluating an activity classifier

func evaluation(on: MLDataTable, featureColumns: [String], labelColumn: String, recordingFileColumn: String) -> MLClassifierMetrics

Generates metrics describing the activity classifier’s performance on labeled activities in a data table.

Deprecated

