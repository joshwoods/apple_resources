

- Create ML
- MLActionClassifier
-  train(trainingData:parameters:sessionParameters:) 

Type Method

# train(trainingData:parameters:sessionParameters:)

Begins an asynchronous action classifier training session.

macOS 11.0+

``` source
static func train(
    trainingData: MLActionClassifier.DataSource,
    parameters: MLActionClassifier.ModelParameters = ModelParameters(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Return Value

An MLJob that represents the action classifier training session.

## Discussion

- trainingData: A collection of labeled videos represented by a data source.

- sessionParameters: An MLTrainingSessionParameters instance you use to configure the training session.

## See Also

### Training an action classifier asynchronously

static func makeTrainingSession(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier.

static func resume(MLTrainingSession&lt;MLActionClassifier>) throws -> MLJob&lt;MLActionClassifier>

Begins or continues an asynchronous action classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier by restoring an existing training session’s state from its parameters.

