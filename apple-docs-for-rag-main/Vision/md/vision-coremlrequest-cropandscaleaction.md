

- Vision
- CoreMLRequest
-  cropAndScaleAction 

Instance Property

# cropAndScaleAction

An optional setting that tells the Vision algorithm how to scale an input image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var cropAndScaleAction: ImageCropAndScaleAction
```

## Discussion

Scaling an image ensures that the entire image fits into the algorithm’s input image dimensions, which may require a change in aspect ratio. The default value is ImageCropAndScaleAction.scaleToFill.

## See Also

### Inspecting a request

var supportedIdentifiers: [String]?

The classification identifiers supported by the request.

let modelContainer: CoreMLModelContainer

The model to base the image analysis request on.

struct CoreMLModelContainer

A model container to use with an image-analysis request.

enum ComputeStage

Types that represent the compute stage.

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

