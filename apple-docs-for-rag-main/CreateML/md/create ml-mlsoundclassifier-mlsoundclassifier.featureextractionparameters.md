

- Create ML
- MLSoundClassifier
-  MLSoundClassifier.FeatureExtractionParameters 

Structure

# MLSoundClassifier.FeatureExtractionParameters

Parameters that affect the process of extracting sound features from audio files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
struct FeatureExtractionParameters
```

## Topics

### Creating feature extraction parameters

init(overlapFactor: Double, featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType, featureExtractionTimeWindowSize: TimeInterval?)

Creates the parameters for a feature-extraction session.

init(overlapFactor: Double, featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType)

Creates the parameters for a feature-extraction session with a default time window size.

### Accessing feature extraction parameters

var overlapFactor: Double

The proportion of overlap that the feature-extraction session uses to analyze two consecutive windows in the audio data.

var featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType

The algorithm type the session uses to extract features from audio files.

var featureExtractionTimeWindowSize: TimeInterval

A time duration, in seconds, that determines how much audio data the feature-extraction session reads each time it samples an audio file.

## Relationships

### Conforms To

- Sendable

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

static func extractFeatures(trainingData: MLSoundClassifier.DataSource, parameters: MLSoundClassifier.FeatureExtractionParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLSoundClassifier.DataSource>

Begins an asynchronous session that extracts sound features from a data source of sound files.

