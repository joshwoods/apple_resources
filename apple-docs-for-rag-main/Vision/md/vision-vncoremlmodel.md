

- Vision
-  VNCoreMLModel 

Class

# VNCoreMLModel

A container for the model to use with Vision requests.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNCoreMLModel
```

## Overview

A Core ML model encapsulates the information trained from a data set used to drive Vision recognition requests. See Getting a Core ML Model for instructions on training your own model. Once you train the model, use this class to initialize a VNCoreMLRequest for identification.

## Topics

### Initializing a Model

convenience init(for: MLModel) throws

Creates a model container to use with a Core ML request.

### Providing Features

var featureProvider: (any MLFeatureProvider)?

An optional object to support inputs outside Vision.

var inputImageFeatureName: String

The name of the feature value that Vision sets from the request handler.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Initializing with a Core ML Model

convenience init(model: VNCoreMLModel)

Creates a model container to use with an image analysis request based on the model you provide.

init(model: VNCoreMLModel, completionHandler: VNRequestCompletionHandler?)

Creates a model container to use with an image analysis request based on the model you provide, with an optional completion handler.

var model: VNCoreMLModel

The model to base the image analysis request on.

