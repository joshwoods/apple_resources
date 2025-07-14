

- Create ML
- MLStyleTransfer
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Creates an asynchronous training session for a style transfer model by restoring an existing training session’s state from its parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Return Value

An MLTrainingSession that represents the style transfer model-training session.

## Discussion

- sessionParameters: The MLTrainingSessionParameters instance you used to create the training session using makeTrainingSession(trainingData:parameters:sessionParameters:).

## See Also

### Training a style transfer model asynchronously

static func train(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLStyleTransfer>

Begins an asynchronous style transfer model-training session.

static func makeTrainingSession(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLStyleTransfer>

Creates an asynchronous training session for a style transfer model.

static func resume(MLTrainingSession&lt;MLStyleTransfer>) throws -> MLJob&lt;MLStyleTransfer>

Begins or continues an asynchronous style transfer model-training session.

