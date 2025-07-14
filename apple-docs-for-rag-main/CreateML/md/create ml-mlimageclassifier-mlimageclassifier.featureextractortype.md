

- Create ML
- MLImageClassifier
-  MLImageClassifier.FeatureExtractorType 

Enumeration

# MLImageClassifier.FeatureExtractorType

The underlying base model that extracts image features for image classifier training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
enum FeatureExtractorType
```

## Overview

Create ML has one built-in feature extractor: `scenePrint`. Alternatively, you can provide your own custom feature extractor from an `.mlmodel` file or a specific layer within a model file.

## Topics

### Selecting a feature extractor type

case scenePrint(revision: Int?)

A feature extractor trained on millions of images.

case custom(MLImageClassifier.CustomFeatureExtractor)

A feature extractor that you provide as a Core ML model file or a layer within that file.

struct CustomFeatureExtractor

A custom feature extractor a training session uses to train an image classifier.

### Describing a feature extractor type

var description: String

A text representation of the feature extractor.

var debugDescription: String

A text representation of the feature extractor that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the feature extractor shown in a playground.

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
- Sendable

## See Also

### Supporting types

enum ValidationData

The source of a validation dataset for an image classifier.

struct ImageAugmentationOptions

The variations that the training process can use to generate more training data from the training data you provide.

