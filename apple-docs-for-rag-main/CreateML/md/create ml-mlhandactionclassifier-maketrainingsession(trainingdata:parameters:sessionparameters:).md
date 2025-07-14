

- Create ML
- MLHandActionClassifier
-  makeTrainingSession(trainingData:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:parameters:sessionParameters:)

Creates an asynchronous hand action classifier’s training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func makeTrainingSession(
    trainingData: MLHandActionClassifier.DataSource,
    parameters: MLHandActionClassifier.ModelParameters = .init(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLTrainingSession
```

## Parameters 

`trainingData`  

An MLHandActionClassifier.DataSource instance.

## Return Value

An MLTrainingSession that represents the action classifier training session.

## Discussion

- sessionParameters: An MLTrainingSessionParameters instance you use to configure the training session.

## See Also

### Training a hand action classifier asynchronously

static func train(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandActionClassifier>

Begins an asynchronous hand action classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandActionClassifier>) throws -> MLJob&lt;MLHandActionClassifier>

Begins or continues an asynchronous hand action classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Recreates an asynchronous hand action classifier’s training session by restoring its saved state from the file system.

