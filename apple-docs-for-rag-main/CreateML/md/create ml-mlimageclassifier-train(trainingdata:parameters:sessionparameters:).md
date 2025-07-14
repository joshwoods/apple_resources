

- Create ML
- MLImageClassifier
-  train(trainingData:parameters:sessionParameters:) 

Type Method

# train(trainingData:parameters:sessionParameters:)

Begins an asynchronous image classifier training session with a training dataset represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func train(
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
) throws -> MLJob
```

## Parameters 

`trainingData`  

Data source for training.

`parameters`  

Model training parameters. See `MLImageClassifier.ModelParameters` for the defaults.

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

An MLJob that represents the image classifier training session.

## See Also

### Training an image classifier asynchronously

static func makeTrainingSession(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates or restores a training session.

static func resume(MLTrainingSession&lt;MLImageClassifier>) throws -> MLJob&lt;MLImageClassifier>

Begins or continues an asynchronous image classifier training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLImageClassifier>

Creates an asynchronous training session for an image classifier by restoring an existing training session’s state from its parameters.

