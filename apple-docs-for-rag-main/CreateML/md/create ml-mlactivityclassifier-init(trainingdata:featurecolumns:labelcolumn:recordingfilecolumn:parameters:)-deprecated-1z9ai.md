

- Create ML
- MLActivityClassifier
-  init(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:) Deprecated

Initializer

# init(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:)

Creates an activity classifier with a training dataset represented by a data table.

macOS 10.15–14.0Deprecated

``` source
init(
    trainingData: MLDataTable,
    featureColumns: [String],
    labelColumn: String,
    recordingFileColumn: String,
    parameters: MLActivityClassifier.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use init(trainingData:parameters:)

## Parameters 

`trainingData`  

An MLDataTable that contains a collection of sensor data that groups data entries by activity label.

`featureColumns`  

The names of the columns in the data table that contain sensor data.

`labelColumn`  

The name of the column in the data table that contains activity labels.

`recordingFileColumn`  

The name of the column in the data table that contains data filenames.

`parameters`  

An MLActivityClassifier.ModelParameters instance you use to configure the model for the training session.

## Discussion

Use this initializer to create an activity classifier with an MLDataTable. To configure the training process, initialize the activity classifier with an MLActivityClassifier.ModelParameters instance. For example, you can explicitly define the validation dataset instead of allowing the model to choose a random selection of your training data. Alternatively, set validationData to `nil` to allow the activity classifier to choose the validation data for you from among your training data. This lets you set other parameters — like maximumIterations and batchSize — to nondefault values.

## See Also

### Training an activity classifier synchronously

init(trainingData: MLActivityClassifier.DataSource, featureColumns: [String], labelColumn: String?, recordingFileColumn: String?, parameters: MLActivityClassifier.ModelParameters) throws

Creates an activity classifier with a training dataset represented by a data source.

