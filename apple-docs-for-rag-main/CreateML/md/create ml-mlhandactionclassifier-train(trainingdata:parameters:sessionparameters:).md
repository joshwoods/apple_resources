

- Create ML
- MLHandActionClassifier
-  train(trainingData:parameters:sessionParameters:) 

Type Method

# train(trainingData:parameters:sessionParameters:)

Begins an asynchronous hand action classifier’s training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func train(
    trainingData: MLHandActionClassifier.DataSource,
    parameters: MLHandActionClassifier.ModelParameters = ModelParameters(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Parameters 

`trainingData`  

An MLHandActionClassifier.DataSource instance.

`parameters`  

An MLHandActionClassifier.ModelParameters instance you use to configure the model for the training session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the training session.

## Return Value

An MLJob that represents the hand action classifier’s training session.

## See Also

### Training a hand action classifier asynchronously

static func makeTrainingSession(trainingData: MLHandActionClassifier.DataSource, parameters: MLHandActionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Creates an asynchronous hand action classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandActionClassifier>) throws -> MLJob&lt;MLHandActionClassifier>

Begins or continues an asynchronous hand action classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandActionClassifier>

Recreates an asynchronous hand action classifier’s training session by restoring its saved state from the file system.

