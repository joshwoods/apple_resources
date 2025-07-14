

- Create ML Components
- ImageFeaturePrint
-  init(revision:cropAndScale:context:) 

Initializer

# init(revision:cropAndScale:context:)

Creates a FeaturePrint feature extractor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    revision: Int,
    cropAndScale: VNImageCropAndScaleOption = .centerCrop,
    context: CIContext = CIContext()
)
```

## Parameters 

`revision`  

The revision of feature extractor to use.

`cropAndScale`  

The scaling and cropping options.

`context`  

The CoreImage context to use for the operation. Defaults to a new default context.

## See Also

### Creating the extractor

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(cropAndScale: VNImageCropAndScaleOption, context: CIContext)

Creates a FeaturePrint feature extractor.

