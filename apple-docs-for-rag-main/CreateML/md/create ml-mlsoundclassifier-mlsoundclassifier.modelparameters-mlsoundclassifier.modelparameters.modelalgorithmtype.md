

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  MLSoundClassifier.ModelParameters.ModelAlgorithmType 

Enumeration

# MLSoundClassifier.ModelParameters.ModelAlgorithmType

The algorithm options to train a sound classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum ModelAlgorithmType
```

## Topics

### Designating an algorithm

case transferLearning(featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType, classifier: MLSoundClassifier.ModelParameters.ClassifierType)

An algorithm that leverages the knowledge of a general-purpose model built into the operating system.

enum FeatureExtractorType

The feature-extractor options for a sound-classifier training algorithm.

enum ClassifierType

The classifier options for a sound classifier training algorithm.

### Describing an algorithm

var description: String

A text representation of the training algorithm.

### Comparing algorithms

static func == (MLSoundClassifier.ModelParameters.ModelAlgorithmType, MLSoundClassifier.ModelParameters.ModelAlgorithmType) -> Bool

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

### Supporting types

enum ValidationData

The source of a validation dataset for a sound classifier.

