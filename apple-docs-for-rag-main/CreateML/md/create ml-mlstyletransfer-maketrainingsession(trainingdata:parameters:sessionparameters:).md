

- Create ML
- MLStyleTransfer
-  makeTrainingSession(trainingData:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:parameters:sessionParameters:)

Creates an asynchronous training session for a style transfer model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func makeTrainingSession(
    trainingData: MLStyleTransfer.DataSource,
    parameters: MLStyleTransfer.ModelParameters = .init(),
    sessionParameters: MLTrainingSessionParameters = .init()
) throws -> MLTrainingSession
```

## Return Value

An MLTrainingSession that represents the style transfer model-training session.

## Discussion

- trainingData: The style image and content images represented by a data source.

- sessionParameters: An MLTrainingSessionParameters instance you use to configure the training session.

## See Also

### Training a style transfer model asynchronously

static func train(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLStyleTransfer>

Begins an asynchronous style transfer model-training session.

static func resume(MLTrainingSession&lt;MLStyleTransfer>) throws -> MLJob&lt;MLStyleTransfer>

Begins or continues an asynchronous style transfer model-training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLStyleTransfer>

Creates an asynchronous training session for a style transfer model by restoring an existing training session’s state from its parameters.

