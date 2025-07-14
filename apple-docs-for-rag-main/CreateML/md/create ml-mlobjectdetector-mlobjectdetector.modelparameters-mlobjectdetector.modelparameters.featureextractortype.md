

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  MLObjectDetector.ModelParameters.FeatureExtractorType 

Enumeration

# MLObjectDetector.ModelParameters.FeatureExtractorType

The underlying base model that extracts image features for an object-detector training session.

macOS 11.0+

``` source
enum FeatureExtractorType
```

## Topics

### Designating a feature extractor

case objectPrint(revision: Int)

A feature extractor you use with a transfer-learning algorithm for object detectors.

## Relationships

### Conforms To

- Sendable

## See Also

### Designating an algorithm

case darknetYolo

An algorithm that trains a full neural network with your training data.

case transferLearning(MLObjectDetector.ModelParameters.FeatureExtractorType)

An algorithm that leverages the knowledge of a general purpose model built into the operating system.

