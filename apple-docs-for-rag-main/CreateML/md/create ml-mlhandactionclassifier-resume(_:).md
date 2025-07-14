

- Create ML
- MLHandActionClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous hand action classifier’s training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Return Value

An MLJob that represents the hand action training session.

## Discussion

- session: An MLTrainingSession instance that represents the training session.

## See Also

### Training a hand action classifier asynchronously

static func train(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandActionClassifier>

Begins an asynchronous hand action classifier’s training session.

static func makeTrainingSession(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Creates an asynchronous hand action classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Recreates an asynchronous hand action classifier’s training session by restoring its saved state from the file system.

