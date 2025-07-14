

- Create ML
- MLSoundClassifier
-  train(trainingData:parameters:sessionParameters:) 

Type Method

# train(trainingData:parameters:sessionParameters:)

Begins an asynchronous sound classifier training session with a training dataset represented by a data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func train(
    trainingData: MLSoundClassifier.DataSource,
    parameters: MLSoundClassifier.ModelParameters = ModelParameters(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Parameters 

`trainingData`  

A collection of labeled audio files represented by an MLSoundClassifier.DataSource.

`parameters`  

An MLSoundClassifier.ModelParameters instance you use to configure the model for the training session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the training session.

## Return Value

An MLJob that represents the sound classifier training session.

## See Also

### Training a sound classifier asynchronously

static func train(trainingData: [String : [URL]], parameters: MLSoundClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLSoundClassifier>

Begins an asynchronous sound classifier training session with a training dataset represented by a dictionary.

static func makeTrainingSession(trainingData: MLSoundClassifier.DataSource, parameters: MLSoundClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLSoundClassifier>

Creates an asynchronous training session for a sound classifier.

static func resume(MLTrainingSession&lt;MLSoundClassifier>) throws -> MLJob&lt;MLSoundClassifier>

Begins or continues an asynchronous training session for a sound classifier.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLSoundClassifier>

Creates an asynchronous training session for a sound classifier by restoring an existing training session’s state from its parameters.

static func extractFeatures(trainingData: MLSoundClassifier.DataSource, parameters: MLSoundClassifier.FeatureExtractionParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLSoundClassifier.DataSource>

Begins an asynchronous session that extracts sound features from a data source of sound files.

struct FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

