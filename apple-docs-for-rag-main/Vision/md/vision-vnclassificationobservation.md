

- Vision
-  VNClassificationObservation 

Class

# VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNClassificationObservation
```

## Overview

This type of observation results from performing a VNCoreMLRequest image analysis with a Core ML model whose role is classification (rather than prediction or image-to-image processing). Vision infers that an MLModel object is a classifier model if that model predicts a single feature. That is, the model’s modelDescription object has a non-`nil` value for its predictedFeatureName property.

## Topics

### Determining Classification

var identifier: String

Classification label identifying the type of observation.

### Measuring Confidence and Precision

var hasPrecisionRecallCurve: Bool

A Boolean variable indicating whether the observation contains precision and recall curves.

func hasMinimumPrecision(Float, forRecall: Float) -> Bool

Determines whether the observation for a specific recall has a minimum precision value.

func hasMinimumRecall(Float, forPrecision: Float) -> Bool

Determines whether the observation for a specific precision has a minimum recall value.

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

class VNPixelBufferObservation

An object that represents an image that an image-analysis request produces.

class VNCoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

