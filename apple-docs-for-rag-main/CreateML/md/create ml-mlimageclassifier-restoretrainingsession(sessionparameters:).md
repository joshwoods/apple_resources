

- Create ML
- MLImageClassifier
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Creates an asynchronous training session for an image classifier by restoring an existing training session’s state from its parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Parameters 

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

An MLTrainingSession that represents the image classifier training session.

## See Also

### Training an image classifier asynchronously

static func makeTrainingSession(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates or restores a training session.

static func train(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLImageClassifier>

Begins an asynchronous image classifier training session with a training dataset represented by a data source.

static func resume(MLTrainingSession&lt;MLImageClassifier>) throws -> MLJob&lt;MLImageClassifier>

Begins or continues an asynchronous image classifier training session.

