

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  MLSoundClassifier.ModelParameters.ClassifierType 

Enumeration

# MLSoundClassifier.ModelParameters.ClassifierType

The classifier options for a sound classifier training algorithm.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum ClassifierType
```

## Topics

### Designating an algorithm’s classifier

case logisticRegressor

A statistical model that uses logistic regression to classify an input vector into a category.

case multilayerPerceptron(layerSizes: [Int])

A neural network model that uses three or more layers to classify an input into a category.

### Describing a classifier type

var description: String

A text representation of the classifier type.

### Comparing a classifier type

static func == (MLSoundClassifier.ModelParameters.ClassifierType, MLSoundClassifier.ModelParameters.ClassifierType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Designating an algorithm

case transferLearning(featureExtractor: MLSoundClassifier.ModelParameters.FeatureExtractorType, classifier: MLSoundClassifier.ModelParameters.ClassifierType)

An algorithm that leverages the knowledge of a general-purpose model built into the operating system.

enum FeatureExtractorType

The feature-extractor options for a sound-classifier training algorithm.

