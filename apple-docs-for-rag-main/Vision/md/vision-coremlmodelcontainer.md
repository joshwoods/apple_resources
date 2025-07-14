

- Vision
-  CoreMLModelContainer 

Structure

# CoreMLModelContainer

A model container to use with an image-analysis request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct CoreMLModelContainer
```

## Topics

### Creating a model container

init(model: MLModel, featureProvider: (any MLFeatureProvider)?) throws

### Getting the feature name

var inputImageFeatureName: String

The name of the feature value that Vision sets from the request handler.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a request

var supportedIdentifiers: [String]?

The classification identifiers supported by the request.

let modelContainer: CoreMLModelContainer

The model to base the image analysis request on.

enum ComputeStage

Types that represent the compute stage.

var cropAndScaleAction: ImageCropAndScaleAction

An optional setting that tells the Vision algorithm how to scale an input image.

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

