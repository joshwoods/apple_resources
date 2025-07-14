

- Create ML
- MLHandPoseClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Begins or continues an asynchronous hand pose classifier’s training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Parameters 

`session`  

An MLTrainingSession instance that represents the training session.

## Return Value

An MLJob that represents the hand pose training session.

## See Also

### Training a hand pose classifier asynchronously

static func train(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandPoseClassifier>

Begins an asynchronous hand pose classifier’s training session.

static func makeTrainingSession(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandPoseClassifier>

Creates an asynchronous hand pose classifier’s training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandPoseClassifier>

Recreates an asynchronous hand pose classifier’s training session by restoring its saved state from the file system.

