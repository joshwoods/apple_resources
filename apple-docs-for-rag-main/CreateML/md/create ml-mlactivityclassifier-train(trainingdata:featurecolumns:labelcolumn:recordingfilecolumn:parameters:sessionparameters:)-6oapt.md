

- Create ML
- MLActivityClassifier
-  train(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:) 

Type Method

# train(trainingData:featureColumns:labelColumn:recordingFileColumn:parameters:sessionParameters:)

Begins an asynchronous activity classifier training session with a training dataset represented by a data source.

macOS 11.0+

``` source
static func train(
    trainingData: MLActivityClassifier.DataSource,
    featureColumns: [String],
    labelColumn: String,
    recordingFileColumn: String,
    parameters: MLActivityClassifier.ModelParameters = ModelParameters(validationData: nil),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Parameters 

`trainingData`  

An MLActivityClassifier.DataSource instance.

`featureColumns`  

The names of the columns in an annotation file that contain sensor data.

`labelColumn`  

The name of the column in an annotation file that contains the activity labels if `trainingData` uses MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

The initializer ignores this parameter if `trainingData` uses MLActivityClassifier.DataSource.labeledDirectories(at:).

`recordingFileColumn`  

The name of the column in an annotation file that contains the data filenames if `trainingData` uses MLActivityClassifier.DataSource.directoryWithDataAndAnnotation(at:annotationFileName:timeStampColumn:labelStartTimeColumn:labelEndTimeColumn:).

The initializer ignores this parameter if `trainingData` uses MLActivityClassifier.DataSource.labeledDirectories(at:).

`parameters`  

An MLActivityClassifier.ModelParameters instance you use to configure the model for the training session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the training session.

## Return Value

An MLJob that represents the activity classifier training session.

## See Also

### Training an activity classifier asynchronously

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

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActivityClassifier>

Creates an asynchronous training session for an activity classifier by restoring an existing training session’s state from its parameters.

