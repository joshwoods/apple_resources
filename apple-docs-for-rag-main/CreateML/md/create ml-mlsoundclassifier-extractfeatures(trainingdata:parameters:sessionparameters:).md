

- Create ML
- MLSoundClassifier
-  extractFeatures(trainingData:parameters:sessionParameters:) 

Type Method

# extractFeatures(trainingData:parameters:sessionParameters:)

Begins an asynchronous session that extracts sound features from a data source of sound files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
static func extractFeatures(
    trainingData: MLSoundClassifier.DataSource,
    parameters: MLSoundClassifier.FeatureExtractionParameters = FeatureExtractionParameters(),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Parameters 

`trainingData`  

An MLSoundClassifier.DataSource instance that contains a collection of labeled audio files.

`parameters`  

An MLSoundClassifier.FeatureExtractionParameters instance you use to configure the feature extraction session.

`sessionParameters`  

An MLTrainingSessionParameters instance you use to configure the feature extraction session.

## Return Value

An MLJob that represents the sound feature extraction session.

## Discussion

Use this method to reduce the training time for multiple sound classifiers that use the same training data. Use the MLJob instance this method returns to save the audio features as an MLSoundClassifier.DataSource. Then use the audio features data source to train one or more sound classifiers.

You can also create a data source from a DataFrame or an MLDataTable that contains audio features by using MLSoundClassifier.DataSource.featuresDataFrame(_:featureColumn:labelColumn:parameters:) or MLSoundClassifier.DataSource.features(table:featureColumn:labelColumn:parameters:), respectively.

## See Also

### Training a sound classifier asynchronously

static func train(trainingData: MLSoundClassifier.DataSource, parameters: MLSoundClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLSoundClassifier>

Begins an asynchronous sound classifier training session with a training dataset represented by a data source.

static func train(trainingData: [String : [URL]], parameters: MLSoundClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLSoundClassifier>

Begins an asynchronous sound classifier training session with a training dataset represented by a dictionary.

static func makeTrainingSession(trainingData: MLSoundClassifier.DataSource, parameters: MLSoundClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLSoundClassifier>

Creates an asynchronous training session for a sound classifier.

static func resume(MLTrainingSession&lt;MLSoundClassifier>) throws -> MLJob&lt;MLSoundClassifier>

Begins or continues an asynchronous training session for a sound classifier.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLSoundClassifier>

Creates an asynchronous training session for a sound classifier by restoring an existing training session’s state from its parameters.

struct FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

