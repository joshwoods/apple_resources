

- Create ML
- MLActivityClassifier
-  train(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:) Deprecated

Type Method

# train(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:)

Begins an asynchronous activity classifier training session with a training dataset represented by a data table.

macOS 11.0–14.0Deprecated

``` source
static func train(
    trainingData: MLDataTable,
    featureColumns: [String],
    labelColumn: String,
    recordingFileColumn: String,
    parameters: MLActivityClassifier.ModelParameters = ModelParameters(validationData: nil),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

Deprecated

Use train(trainingData:parameters:sessionParameters:)

## Parameters 

`trainingData`  

An MLDataTable instance that contains a collection of sensor data that groups data entries by activity label.

`featureColumns`  

The names of the columns in the data table that contain sensor data.

`labelColumn`  

The name of the column in the data table that contains activity labels.

`recordingFileColumn`  

The name of the column in the data table that contains data filenames.

`parameters`  

An MLActivityClassifier.ModelParameters instance you use to configure the model for the training session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the training session.

## Return Value

An MLJob that represents the activity classifier training session.

## See Also

### Training an activity classifier asynchronously

static func train(trainingData: MLActivityClassifier.DataSource, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActivityClassifier>

Begins an asynchronous activity classifier training session with a training dataset represented by a data source.

static func makeTrainingSession(trainingData: MLDataTable, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier.

Deprecated

static func makeTrainingSession(trainingData: MLActivityClassifier.DataSource, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier.

static func resume(MLTrainingSession&lt;MLActivityClassifier>) throws -> MLJob&lt;MLActivityClassifier>

Begins or continues an asynchronous activity classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier by restoring an existing training session’s state from its parameters.

