

- Vision
- GenerateImageFeaturePrintRequest
-  cropAndScaleAction 

Instance Property

# cropAndScaleAction

An optional setting that tells the algorithm how to scale an input image before generating the result.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var cropAndScaleAction: ImageCropAndScaleAction
```

## Discussion

The system applies scaling before generating the feature print. The default value is ImageCropAndScaleAction.scaleToFill.

## See Also

### Inspecting a request

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

