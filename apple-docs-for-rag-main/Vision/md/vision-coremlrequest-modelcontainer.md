

- Vision
- CoreMLRequest
-  modelContainer 

Instance Property

# modelContainer

The model to base the image analysis request on.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let modelContainer: CoreMLModelContainer
```

## Discussion

This object wraps a Core ML model.

## See Also

### Inspecting a request

var supportedIdentifiers: [String]?

The classification identifiers supported by the request.

struct CoreMLModelContainer

A model container to use with an image-analysis request.

enum ComputeStage

Types that represent the compute stage.

var cropAndScaleAction: ImageCropAndScaleAction

An optional setting that tells the Vision algorithm how to scale an input image.

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

