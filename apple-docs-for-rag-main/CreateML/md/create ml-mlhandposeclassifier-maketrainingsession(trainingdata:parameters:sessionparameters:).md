

- Create ML
- MLHandPoseClassifier
-  makeTrainingSession(trainingData:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:parameters:sessionParameters:)

Creates an asynchronous hand pose classifier’s training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func makeTrainingSession(
    trainingData: MLHandPoseClassifier.DataSource,
    parameters: MLHandPoseClassifier.ModelParameters = .init(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLTrainingSession
```

## Parameters 

`trainingData`  

An MLHandPoseClassifier.DataSource instance.

`parameters`  

An MLHandPoseClassifier.ModelParameters instance you use to configure the model for the training session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the training session.

## Return Value

An MLTrainingSession that represents the action classifier training session.

## See Also

### Training a hand pose classifier asynchronously

static func train(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandPoseClassifier>

Begins an asynchronous hand pose classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandPoseClassifier>) throws -> MLJob&lt;MLHandPoseClassifier>

Begins or continues an asynchronous hand pose classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandPoseClassifier>

Recreates an asynchronous hand pose classifier’s training session by restoring its saved state from the file system.

