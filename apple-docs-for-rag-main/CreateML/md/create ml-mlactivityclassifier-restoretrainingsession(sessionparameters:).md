

- Create ML
- MLActivityClassifier
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Creates an asynchronous training session for an activity classifier by restoring an existing training session’s state from its parameters.

macOS 11.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Parameters 

`sessionParameters`  

The MLTrainingSessionParameters instance you used to create the training session using `MLActivityClassifier/makeTrainingSession(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:)`.

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

static func makeTrainingSession(trainingData: MLActivityClassifier.DataSource, featureColumns: [String], labelColumn: String, recordingFileColumn: String, parameters: MLActivityClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier.

static func resume(MLTrainingSession&lt;MLActivityClassifier>) throws -> MLJob&lt;MLActivityClassifier>

Begins or continues an asynchronous activity classifier training session.

