

- Create ML
- MLActivityClassifier
-  makeTrainingSession(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:)

Creates an asynchronous training session for an activity classifier.

macOS 14.0+

``` source
static func makeTrainingSession(
    trainingData: MLActivityClassifier.DataSource,
    featureColumns: [String],
    labelColumn: String,
    recordingFileColumn: String,
    parameters: MLActivityClassifier.ModelParameters = .init(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLTrainingSession
```

## Parameters 

`trainingData`  

An MLDataTable instance that contains a collection of sensor data that groups data entries by activity label.

`featureColumns`  

The feature column names.

`labelColumn`  

The label column name,

`recordingFileColumn`  

The recording file column name.

`parameters`  

An MLActivityClassifier.ModelParameters instance you use to configure the model for the training session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the training session.

## Return Value

An MLTrainingSession that represents the activity classifier training session.

## See Also

### Training an activity classifier asynchronously

static func train(trainingData: MLActivityClassifier.DataSource, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActivityClassifier>

Begins an asynchronous activity classifier training session with a training dataset represented by a data source.

static func train(trainingData: MLDataTable, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActivityClassifier>

Begins an asynchronous activity classifier training session with a training dataset represented by a data table.

Deprecated

static func makeTrainingSession(trainingData: MLDataTable, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier.

Deprecated

static func resume(MLTrainingSession&lt;MLActivityClassifier>) throws -> MLJob&lt;MLActivityClassifier>

Begins or continues an asynchronous activity classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier by restoring an existing training session’s state from its parameters.

