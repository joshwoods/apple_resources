

- Vision
- CoreMLRequest
-  supportedIdentifiers 

Instance Property

# supportedIdentifiers

The classification identifiers supported by the request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var supportedIdentifiers: [String]? { get }
```

## Discussion

This returns `nil` if the configuration isn’t supported.

## See Also

### Inspecting a request

let modelContainer: CoreMLModelContainer

The model to base the image analysis request on.

struct CoreMLModelContainer

A model container to use with an image-analysis request.

enum ComputeStage

Types that represent the compute stage.

var cropAndScaleAction: ImageCropAndScaleAction

An optional setting that tells the Vision algorithm how to scale an input image.

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

