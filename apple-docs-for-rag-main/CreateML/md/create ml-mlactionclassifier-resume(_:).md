

- Create ML
- MLActionClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous action classifier training session.

macOS 11.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Return Value

An MLJob that represents the action classifier training session.

## Discussion

- session: An MLTrainingSession instance that represents the training session.

## See Also

### Training an action classifier asynchronously

static func train(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLActionClassifier>

Begins an asynchronous action classifier training session.

static func makeTrainingSession(trainingData: MLActionClassifier.DataSource, parameters: MLActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLActionClassifier>

Creates an asynchronous training session for an action classifier by restoring an existing training session’s state from its parameters.

