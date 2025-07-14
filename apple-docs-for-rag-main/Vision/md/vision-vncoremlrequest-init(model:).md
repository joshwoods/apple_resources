

- Vision
- VNCoreMLRequest
-  init(model:) 

Initializer

# init(model:)

Creates a model container to use with an image analysis request based on the model you provide.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
convenience init(model: VNCoreMLModel)
```

## Parameters 

`model`  

The Core ML model on which to base the Vision request.

## Discussion

Initialization can fail if the Core ML model you provide isn’t supported in Vision, such as if the model doesn’t accept an image as input.

## See Also

### Initializing with a Core ML Model

init(model: VNCoreMLModel, completionHandler: VNRequestCompletionHandler?)

Creates a model container to use with an image analysis request based on the model you provide, with an optional completion handler.

var model: VNCoreMLModel

The model to base the image analysis request on.

class VNCoreMLModel

A container for the model to use with Vision requests.

