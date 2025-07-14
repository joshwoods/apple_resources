

- Create ML
- MLImageClassifier
-  makeTrainingSession(trainingData:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:parameters:sessionParameters:)

Creates or restores a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func makeTrainingSession(
    trainingData: MLImageClassifier.DataSource,
    parameters: MLImageClassifier.ModelParameters = ModelParameters(
            validation: .split(strategy: .automatic),
            augmentation: [],
            algorithm: .transferLearning(
                featureExtractor: .scenePrint(revision: 1),
                classifier: .logisticRegressor
            )
        ),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLTrainingSession
```

## Parameters 

`trainingData`  

Data source for training.

`parameters`  

Model training parameters. See `MLImageClassifier.ModelParameters` for the defaults.

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

A `MLTrainingSession` that can be used to start or resume training.

## See Also

### Training an image classifier asynchronously

static func train(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLImageClassifier>

Begins an asynchronous image classifier training session with a training dataset represented by a data source.

static func resume(MLTrainingSession&lt;MLImageClassifier>) throws -> MLJob&lt;MLImageClassifier>

Begins or continues an asynchronous image classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates an asynchronous training session for an image classifier by restoring an existing training session’s state from its parameters.

