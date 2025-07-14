

- Create ML
- MLImageClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous image classifier training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Parameters 

`session`  

An MLTrainingSession instance that represents the training session.

## Return Value

An MLJob that represents the image classifier training session.

## See Also

### Training an image classifier asynchronously

static func makeTrainingSession(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates or restores a training session.

static func train(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLImageClassifier>

Begins an asynchronous image classifier training session with a training dataset represented by a data source.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates an asynchronous training session for an image classifier by restoring an existing training session’s state from its parameters.

