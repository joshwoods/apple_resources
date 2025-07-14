

- Create ML
- MLSoundClassifier
-  MLSoundClassifier.ModelParameters 

Structure

# MLSoundClassifier.ModelParameters

Parameters that affect the process of training a sound-classifier model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
struct ModelParameters
```

## Overview

By default, a sound-classifier training session’s transfer-learning algorithm uses the MLSoundClassifier.ModelParameters.FeatureExtractorType.audioFeaturePrint(type:revision:) feature extractor. See MLSoundClassifier.ModelParameters.FeatureExtractorType for more information.

## Topics

### Creating parameters

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double)

Creates a new set of training parameters for a sound classifier with a validation dataset.

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double, algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType)

Creates a new set of training parameters for a sound classifier with a validation dataset and a training algorithm.

init(validation: MLSoundClassifier.ModelParameters.ValidationData, maxIterations: Int, overlapFactor: Double, algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType, featureExtractionTimeWindowSize: TimeInterval)

Creates a new set of training parameters for a sound classifier with a validation dataset, a training algorithm, and a time-window size.

### Accessing the training parameters

var validation: MLSoundClassifier.ModelParameters.ValidationData

The sound classifier’s validation dataset.

var maxIterations: Int

The largest number of iterations the training session can use.

var overlapFactor: Double

The proportion of overlap that the training session uses to analyze two consecutive windows in the audio data.

var algorithm: MLSoundClassifier.ModelParameters.ModelAlgorithmType

The algorithm the training session uses to train the sound classifier.

var featureExtractionTimeWindowSize: TimeInterval

A time duration, in seconds, the training session uses for each audio sample it reads from an audio file in a dataset.

### Describing parameters

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the parameters in a playground.

### Supporting types

enum ValidationData

The source of a validation dataset for a sound classifier.

enum ModelAlgorithmType

The algorithm options to train a sound classifier.

### Enumerations

enum ClassifierType

The classifier options for a sound classifier training algorithm.

enum FeatureExtractorType

The feature-extractor options for a sound-classifier training algorithm.

enum FeaturePrintType

The type options for an Audio Feature Print feature extractor.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible

## See Also

### Supporting types

enum DataSource

A representation of a sound-classifier dataset located in the file system or in a data table.

