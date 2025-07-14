

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  MLObjectDetector.ModelParameters.ModelAlgorithmType 

Enumeration

# MLObjectDetector.ModelParameters.ModelAlgorithmType

An object-detector training algorithm.

macOS 11.0+

``` source
enum ModelAlgorithmType
```

## Topics

### Designating an algorithm

case darknetYolo

An algorithm that trains a full neural network with your training data.

case transferLearning(MLObjectDetector.ModelParameters.FeatureExtractorType)

An algorithm that leverages the knowledge of a general purpose model built into the operating system.

enum FeatureExtractorType

The underlying base model that extracts image features for an object-detector training session.

### Comparing algorithms

static func == (MLObjectDetector.ModelParameters.ModelAlgorithmType, MLObjectDetector.ModelParameters.ModelAlgorithmType) -> Bool

Returns a Boolean value that indicates whether two algorithm are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Supporting types

enum ValidationData

A validation dataset for an object detector.

