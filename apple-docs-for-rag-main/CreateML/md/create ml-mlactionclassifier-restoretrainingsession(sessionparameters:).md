

- Create ML
- MLActionClassifier
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Creates an asynchronous training session for an action classifier by restoring an existing training session’s state from its parameters.

macOS 11.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Return Value

An MLTrainingSession that represents the action classifier training session.

## Discussion

- sessionParameters: The MLTrainingSessionParameters instance you used to create the training session using makeTrainingSession(trainingData:parameters:sessionParameters:).

## See Also

### Training an action classifier asynchronously

static func train(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActionClassifier>

Begins an asynchronous action classifier training session.

static func makeTrainingSession(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier.

static func resume(MLTrainingSession&lt;MLActionClassifier>) throws -> MLJob&lt;MLActionClassifier>

Begins or continues an asynchronous action classifier training session.

