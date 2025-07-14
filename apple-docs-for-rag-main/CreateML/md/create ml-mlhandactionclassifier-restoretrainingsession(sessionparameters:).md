

- Create ML
- MLHandActionClassifier
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Recreates an asynchronous hand action classifier’s training session by restoring its saved state from the file system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Return Value

An MLTrainingSession that represents the hand action classifier training session.

## Discussion

- sessionParameters: The same MLTrainingSessionParameters instance that created an existing training session.

## See Also

### Training a hand action classifier asynchronously

static func train(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandActionClassifier>

Begins an asynchronous hand action classifier’s training session.

static func makeTrainingSession(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Creates an asynchronous hand action classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandActionClassifier>) throws -> MLJob&lt;MLHandActionClassifier>

Begins or continues an asynchronous hand action classifier’s training session.

