

- Vision
-  CoreMLFeatureValueObservation 

Structure

# CoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct CoreMLFeatureValueObservation
```

## Overview

This type of observation results from performing a CoreMLRequest image analysis with a Core ML model whose role is prediction rather than classification or image-to-image processing.

The framework infers that an MLModel object is a predictor model if that model predicts multiple features. You can tell that a model predicts multiple features when its modelDescription object has a `nil` value for its predictedFeatureName property, or when it inserts its output in an outputDescriptionsByName dictionary.

The confidence for these observations is always `1.0`.

## Topics

### Creating an observation

init?(VNCoreMLFeatureValueObservation)

Creates a feature value observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

### Getting the feature name and value

let featureName: String

The name in the model description of the model that produces this observation.

let featureValue: MLSendableFeatureValue

The feature result of a request that outputs neither a classification nor an image.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- VisionObservation

## See Also

### Machine learning image analysis

struct CoreMLRequest

An image-analysis request that uses a Core ML model to process images.

struct ClassificationObservation

An object that represents classification information that an image-analysis request produces.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

