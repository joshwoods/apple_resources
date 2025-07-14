

- Vision
- VNCoreMLRequest
-  init(model:completionHandler:) 

Initializer

# init(model:completionHandler:)

Creates a model container to use with an image analysis request based on the model you provide, with an optional completion handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    model: VNCoreMLModel,
    completionHandler: VNRequestCompletionHandler? = nil
)
```

## Parameters 

`model`  

The Core ML model on which to base the Vision request.

`completionHandler`  

An optional block of code to execute after model initialization.

## Discussion

Initialization can fail if the Core ML model you provide isn’t supported in Vision, such as if the model doesn’t accept an image as input.

## See Also

### Initializing with a Core ML Model

convenience init(model: VNCoreMLModel)

Creates a model container to use with an image analysis request based on the model you provide.

var model: VNCoreMLModel

The model to base the image analysis request on.

class VNCoreMLModel

A container for the model to use with Vision requests.

