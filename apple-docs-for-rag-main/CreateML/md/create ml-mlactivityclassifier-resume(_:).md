

- Create ML
- MLActivityClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous activity classifier training session.

macOS 11.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Parameters 

`session`  

An MLTrainingSession instance that represents the training session.

## Return Value

An MLJob that represents the activity classifier training session.

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

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier by restoring an existing training session’s state from its parameters.

