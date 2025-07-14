

- Core Image
- CIRAWFilter
-  boostAmount 

Instance Property

# boostAmount

A value that indicates the amount of global tone curve to apply to the image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var boostAmount: Float { get set }
```

## Discussion

The value should be in the range of `0...1`. A value of `0` indicates no global tone curve (linear response), and a value of `1` indicates full global tone curve. The default value is `1`.

## See Also

### Configuring a filter

var baselineExposure: Float

A value that indicates the baseline exposure to apply to the image.

var boostShadowAmount: Float

A value that indicates the amount to boost the shadow areas of the image.

var colorNoiseReductionAmount: Float

A value that indicates the amount of chroma noise reduction to apply to the image.

var contrastAmount: Float

A value that indicates the amount of local contrast to apply to the edges of the image.

var decoderVersion: CIRAWDecoderVersion

A value that indicates the decoder version to use.

var detailAmount: Float

A value that indicates the amount of detail enhancement to apply to the edges of the image.

var exposure: Float

A value that indicates the amount of exposure to apply to the image.

var extendedDynamicRangeAmount: Float

A value that indicates the amount of extended dynamic range (EDR) to apply to the image.

var isDraftModeEnabled: Bool

A Boolean that indicates whether to enable draft mode.

var isGamutMappingEnabled: Bool

A Boolean that indicates whether to enable gamut mapping.

var isLensCorrectionEnabled: Bool

A Boolean that indicates whether to enable lens correction.

var linearSpaceFilter: CIFilter?

An optional filter you can apply to the RAW image while it’s in linear space.

var localToneMapAmount: Float

A value that indicates the amount of local tone curve to apply to the image.

var luminanceNoiseReductionAmount: Float

A value that indicates the amount of luminance noise reduction to apply to the image.

var moireReductionAmount: Float

A value that indicates the amount of moire artifact reduction to apply to high frequency areas of the image.

var neutralChromaticity: CGPoint

A value that indicates the amount of white balance based on chromaticity values to apply to the image.

var neutralLocation: CGPoint

A value that indicates the amount of white balance based on pixel coordinates to apply to the image.

var neutralTemperature: Float

A value that indicates the amount of white balance based on temperature values to apply to the image.

var neutralTint: Float

A value that indicates the amount of white balance based on tint values to apply to the image.

var orientation: CGImagePropertyOrientation

A value that indicates the orientation of the image.

var portraitEffectsMatte: CIImage?

An optional auxiliary image that represents the portrait effects matte of the image.

var previewImage: CIImage?

An optional auxiliary image that represents a preview of the original image.

var properties: [AnyHashable : Any]

A dictionary that contains properties of the image source.

var scaleFactor: Float

A value that indicates the desired scale factor to draw the output image.

var semanticSegmentationGlassesMatte: CIImage?

An optional auxiliary image that represents the semantic segmentation glasses matte of the image.

var semanticSegmentationHairMatte: CIImage?

An optional auxiliary image that represents the semantic segmentation hair matte of the image.

var semanticSegmentationSkinMatte: CIImage?

An optional auxiliary image that represents the semantic segmentation skin matte of the image.

var semanticSegmentationSkyMatte: CIImage?

An optional auxiliary image that represents the semantic segmentation sky matte of the image.

var semanticSegmentationTeethMatte: CIImage?

An optional auxiliary image that represents the semantic segmentation teeth matte of the image.

var shadowBias: Float

A value that indicates the amount to subtract from the shadows in the image.

var sharpnessAmount: Float

A value that indicates the amount of sharpness to apply to the edges of the image.

