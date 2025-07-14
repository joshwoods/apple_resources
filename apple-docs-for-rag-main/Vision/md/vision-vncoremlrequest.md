

- Vision
-  VNCoreMLRequest 

Class

# VNCoreMLRequest

An image-analysis request that uses a Core ML model to process images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNCoreMLRequest
```

## Overview

The results array of a Core ML-based image analysis request contains a different observation type, depending on the kind of MLModel object you use:

- If the model predicts a single feature, the model’s modelDescription object has a non-`nil` value for predictedFeatureName and Vision treats the model as a classifier. The results are VNClassificationObservation objects.

- If the model’s outputs include at least one output with a feature type of MLFeatureType.image, Vision treats that model as an image-to-image model. The results are VNPixelBufferObservation objects.

- Otherwise, Vision treats the model as a general predictor model. The results are VNCoreMLFeatureValueObservation objects.

Note

Vision forwards all confidence values from Core ML models as-is and doesn’t normalize them to `[0, 1]`.

## Topics

### Initializing with a Core ML Model

convenience init(model: VNCoreMLModel)

Creates a model container to use with an image analysis request based on the model you provide.

init(model: VNCoreMLModel, completionHandler: VNRequestCompletionHandler?)

Creates a model container to use with an image analysis request based on the model you provide, with an optional completion handler.

var model: VNCoreMLModel

The model to base the image analysis request on.

class VNCoreMLModel

A container for the model to use with Vision requests.

### Configuring Image Options

var imageCropAndScaleOption: VNImageCropAndScaleOption

An optional setting that tells the Vision algorithm how to scale an input image.

enum VNImageCropAndScaleOption

Options that define how Vision crops and scales an input-image.

### Identifying Request Revisions

let VNCoreMLRequestRevision1: Int

A constant for specifying revision 1 of a Core ML request.

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Machine learning image analysis

Classifying Images with Vision and Core ML

Crop and scale photos using the Vision framework and classify them with a Core ML model.

Training a Create ML Model to Classify Flowers

Train a flower classifier using Create ML in Swift Playgrounds, and apply the resulting model to real-time image classification using Vision.

class VNClassificationObservation

An object that represents classification information that an image-analysis request produces.

class VNPixelBufferObservation

An object that represents an image that an image-analysis request produces.

class VNCoreMLFeatureValueObservation

An object that represents a collection of key-value information that a Core ML image-analysis request produces.

