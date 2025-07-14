

- Core Image
- CIRAWFilter
-  isLocalToneMapSupported 

Instance Property

# isLocalToneMapSupported

A Boolean that indicates if the current image supports local tone curve adjustments.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var isLocalToneMapSupported: Bool { get }
```

## Discussion

If this value is `true`, you can adjust the amount of local tone curve to apply to the image by setting localToneMapAmount.

## See Also

### Inspecting supported camera models, decoders, and filters

class var supportedCameraModels: [String]

An array containing the names of all supported camera models.

var supportedDecoderVersions: [CIRAWDecoderVersion]

An array of all supported decoder versions for the given image type.

struct CIRAWDecoderVersion

var isColorNoiseReductionSupported: Bool

A Boolean that indicates if the current image supports color noise reduction adjustments.

var isContrastSupported: Bool

A Boolean that indicates if the current image supports contrast adjustments.

var isDetailSupported: Bool

A Boolean that indicates if the current image supports detail enhancement adjustments.

var isLensCorrectionSupported: Bool

A Boolean that indicates if you can enable lens correction for the current image.

var isLuminanceNoiseReductionSupported: Bool

A Boolean that indicates if the current image supports luminance noise reduction adjustments.

var isMoireReductionSupported: Bool

A Boolean that indicates if the current image supports moire artifact reduction adjustments.

var isSharpnessSupported: Bool

A Boolean that indicates if the current image supports sharpness adjustments.

var nativeSize: CGSize

The full native size of the unscaled image.

