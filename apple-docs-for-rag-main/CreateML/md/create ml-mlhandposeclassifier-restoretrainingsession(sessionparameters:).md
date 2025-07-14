

- Create ML
- MLHandPoseClassifier
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Recreates an asynchronous hand pose classifier’s training session by restoring its saved state from the file system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Parameters 

`sessionParameters`  

The same MLTrainingSessionParameters instance that created an existing training session.

## Return Value

An MLTrainingSession that represents the hand pose classifier training session.

## See Also

### Training a hand pose classifier asynchronously

static func train(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLHandPoseClassifier>

Begins an asynchronous hand pose classifier’s training session.

static func makeTrainingSession(trainingData: MLHandPoseClassifier.DataSource, parameters: MLHandPoseClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLHandPoseClassifier>

Creates an asynchronous hand pose classifier’s training session.

static func resume(MLTrainingSession&lt;MLHandPoseClassifier>) throws -> MLJob&lt;MLHandPoseClassifier>

Begins or continues an asynchronous hand pose classifier’s training session.

