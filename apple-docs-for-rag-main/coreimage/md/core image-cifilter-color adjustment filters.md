

- Core Image
- CIFilter
-  Color Adjustment Filters 

API Collection

# Color Adjustment Filters

## Topics

### Filters

class func colorAbsoluteDifference() -> any CIFilter &amp; CIColorAbsoluteDifference

Calculates the absolute difference between each color component in the input images.

class func colorClamp() -> any CIFilter &amp; CIColorClamp

Alters the colors in an image based on color components.

class func colorControls() -> any CIFilter &amp; CIColorControls

Alters the brightness, contrast, and saturation of an image’s colors.

class func colorMatrix() -> any CIFilter &amp; CIColorMatrix

Alters the colors in an image based on vectors provided.

class func colorPolynomial() -> any CIFilter &amp; CIColorPolynomial

Alters an image’s colors.

class func colorThreshold() -> any CIFilter &amp; CIColorThreshold

Compares the red, green, and blue components of the input image to a threshold and sets them to 1 or 0.

class func colorThresholdOtsu() -> any CIFilter &amp; CIColorThresholdOtsu

Compares the red, green, and blue components of the input image against a threshold calculated using Otsu’s algorithm.

class func depthToDisparity() -> any CIFilter &amp; CIDepthToDisparity

Converts from an image containing depth data to an image containing disparity data.

class func disparityToDepth() -> any CIFilter &amp; CIDisparityToDepth

Creates depth data from an image containing disparity data.

class func exposureAdjust() -> any CIFilter &amp; CIExposureAdjust

Adjusts an image’s exposure.

class func gammaAdjust() -> any CIFilter &amp; CIGammaAdjust

Alters an image’s transition between black and white.

class func hueAdjust() -> any CIFilter &amp; CIHueAdjust

Modifies an image’s hue.

class func linearToSRGBToneCurve() -> any CIFilter &amp; CILinearToSRGBToneCurve

Alters an image’s color intensity.

class func sRGBToneCurveToLinear() -> any CIFilter &amp; CISRGBToneCurveToLinear

Converts the colors in an image from sRGB to linear.

class func temperatureAndTint() -> any CIFilter &amp; CITemperatureAndTint

Alters an image’s temperature and tint.

class func toneCurve() -> any CIFilter &amp; CIToneCurve

Alters an image’s tone curve according to a series of data points.

class func vibrance() -> any CIFilter &amp; CIVibrance

Adjusts an image’s vibrancy.

class func whitePointAdjust() -> any CIFilter &amp; CIWhitePointAdjust

Adjusts the image’s white-point.

### Protocols

protocol CIColorAbsoluteDifference

protocol CIColorClamp

The properties you use to configure a color clamp filter.

protocol CIColorControls

The properties you use to configure a color controls filter.

protocol CIColorMatrix

The properties you use to configure a color matrix filter.

protocol CIColorPolynomial

The properties you use to configure a color polynomial filter.

protocol CIColorThreshold

protocol CIColorThresholdOtsu

protocol CIDepthToDisparity

The properties you use to configure a depth-to-disparity filter.

protocol CIDisparityToDepth

The properties you use to configure a disparity-to-depth filter.

protocol CIExposureAdjust

The properties you use to configure an exposure adjust filter.

protocol CIGammaAdjust

The properties you use to configure a gamma adjust filter.

protocol CIHueAdjust

The properties you use to configure a hue adjust filter.

protocol CILinearToSRGBToneCurve

The properties you use to configure a linear-to-sRGB filter.

protocol CISRGBToneCurveToLinear

The properties you use to configure an sRGB-to-linear filter.

protocol CITemperatureAndTint

The properties you use to configure a temperature and tint filter.

protocol CIToneCurve

The properties you use to configure a tone curve filter.

protocol CIVibrance

The properties you use to configure a vibrance filter.

protocol CIWhitePointAdjust

The properties you use to configure a white-point adjust filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

