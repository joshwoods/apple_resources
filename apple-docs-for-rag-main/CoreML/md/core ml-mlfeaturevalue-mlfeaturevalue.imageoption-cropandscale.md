

- Core ML
- MLFeatureValue
- MLFeatureValue.ImageOption
-  cropAndScale 

Type Property

# cropAndScale

The option you use to crop and scale an image when creating an image feature value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let cropAndScale: MLFeatureValue.ImageOption
```

## Discussion

Use this value as a dictionary key for the `options` argument of an image-based `MLFeatureValue` initializer. Pair this key with a VNImageCropAndScaleOption value in the initializer’s `options` dictionary. For example, see init(CGImage:pixelsWide:pixelsHigh:pixelFormatType:options:).

## See Also

### Image Options Keys

static let cropRect: MLFeatureValue.ImageOption

The option you use to crop an image when creating an image feature value.

