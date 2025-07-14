

- Vision
-  VNCoreMLFeatureValueObservation 

Class

# VNCoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNCoreMLFeatureValueObservation
```

## Overview

This type of observation results from performing a VNCoreMLRequest image analysis with a Core ML model whose role is prediction rather than classification or image-to-image processing.

Vision infers that an MLModel object is a predictor model if that model predicts multiple features. You can tell that a model predicts multiple features when its modelDescription object has a `nil` value for its predictedFeatureName property, or when it inserts its output in an outputDescriptionsByName dictionary.

## Topics

### Obtaining Feature Values

var featureValue: MLFeatureValue

The feature result of a VNCoreMLRequest that outputs neither a classification nor an image.

var featureName: String

The name used in the model description of the CoreML model that produced this observation.

## Relationships

### Inherits From

- VNObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Machine learning image analysis

Classifying Images with Vision and Core ML

Crop and scale photos using the Vision framework and classify them with a Core ML model.

Training a Create ML Model to Classify Flowers

Train a flower classifier using Create ML in Swift Playgrounds, and apply the resulting model to real-time image classification using Vision.

class VNCoreMLRequest

An image-analysis request that uses a Core ML model to process images.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

class VNPixelBufferObservation

An object that represents an image that an image-analysis request produces.

