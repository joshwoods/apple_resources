

- Create ML
- MLStyleTransfer
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous style transfer model-training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Return Value

An MLJob that represents the style transfer model-training session.

## Discussion

- session: An MLTrainingSession instance that represents the training session.

## See Also

### Training a style transfer model asynchronously

static func train(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLStyleTransfer>

Begins an asynchronous style transfer model-training session.

static func makeTrainingSession(trainingData: MLStyleTransfer.DataSource, parameters: MLStyleTransfer.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLStyleTransfer>

Creates an asynchronous training session for a style transfer model.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLStyleTransfer>

Creates an asynchronous training session for a style transfer model by restoring an existing training session’s state from its parameters.

