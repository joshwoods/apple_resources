

- Create ML Components
- ImageFeaturePrint
-  init(cropAndScale:context:) 

Initializer

# init(cropAndScale:context:)

Creates a FeaturePrint feature extractor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    cropAndScale: VNImageCropAndScaleOption = .centerCrop,
    context: CIContext = CIContext()
)
```

## Parameters 

`cropAndScale`  

The scaling and cropping options.

`context`  

The CoreImage context to use for the operation. Defaults to a new default context.

## See Also

### Creating the extractor

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(revision: Int, cropAndScale: VNImageCropAndScaleOption, context: CIContext)

Creates a FeaturePrint feature extractor.

