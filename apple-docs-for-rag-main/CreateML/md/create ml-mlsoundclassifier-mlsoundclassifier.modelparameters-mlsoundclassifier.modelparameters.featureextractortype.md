

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  MLSoundClassifier.ModelParameters.FeatureExtractorType 

Enumeration

# MLSoundClassifier.ModelParameters.FeatureExtractorType

The feature-extractor options for a sound-classifier training algorithm.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum FeatureExtractorType
```

## Overview

Use the MLSoundClassifier.ModelParameters.FeatureExtractorType.audioFeaturePrint(type:revision:) feature extractor to create a model with the following advantages over `vggish`:

- More accurate predictions

- Lower latency

- Smaller model file size

- Less training time

Use MLSoundClassifier.ModelParameters.FeatureExtractorType.vggish(revision:) to support older OS versions.

## Topics

### Designating a feature extractor

case audioFeaturePrint(type: MLSoundClassifier.ModelParameters.FeaturePrintType, revision: Int)

Represents the Audio Feature Print extractor.

enum FeaturePrintType

The type options for an Audio Feature Print feature extractor.

case vggish(revision: Int)

Represents the VGGish feature extractor, which is compatible with older OS versions.

### Describing a feature extractor

var description: String

A text representation of the feature-extractor type.

### Comparing feature extractors

static func == (MLSoundClassifier.ModelParameters.FeatureExtractorType, MLSoundClassifier.ModelParameters.FeatureExtractorType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Designating an algorithm

case transferLearning(featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType, classifier: MLSoundClassifier.ModelParameters.ClassifierType)

An algorithm that leverages the knowledge of a general-purpose model built into the operating system.

enum ClassifierType

The classifier options for a sound classifier training algorithm.

