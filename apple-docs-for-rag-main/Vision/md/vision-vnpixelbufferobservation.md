

- Vision
-  VNPixelBufferObservation 

Class

# VNPixelBufferObservation

An object that represents an image that an image-analysis request produces.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNPixelBufferObservation
```

## Overview

This type of observation results from performing a VNCoreMLRequest image analysis with a Core ML model that has an image-to-image processing role. For example, this observation might result from a model that analyzes the style of one image and then transfers that style to a different image.

Vision infers that an MLModel object is an image-to-image model if that model includes an image. Its modelDescription object includes an image-typed feature description in its outputDescriptionsByName dictionary.

## Topics

### Parsing Observation Content

var pixelBuffer: CVPixelBuffer

The image that results from a request with image output.

var featureName: String?

A feature name that the CoreML model defines.

### Getting the supported pixel formats

func supportedOutputPixelFormats() throws -> [NSNumber]

Returns a list of output pixel formats that the request supports.

## Relationships

### Inherits From

- VNObservation

### Inherited By

- VNSaliencyImageObservation

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

class VNCoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

