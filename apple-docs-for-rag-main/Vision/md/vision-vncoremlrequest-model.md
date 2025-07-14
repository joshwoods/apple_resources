

- Vision
- VNCoreMLRequest
-  model 

Instance Property

# model

The model to base the image analysis request on.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var model: VNCoreMLModel { get }
```

## Discussion

This object wraps a Core ML model.

## See Also

### Initializing with a Core ML Model

convenience init(model: VNCoreMLModel)

Creates a model container to use with an image analysis request based on the model you provide.

init(model: VNCoreMLModel, completionHandler: VNRequestCompletionHandler?)

Creates a model container to use with an image analysis request based on the model you provide, with an optional completion handler.

class VNCoreMLModel

A container for the model to use with Vision requests.

