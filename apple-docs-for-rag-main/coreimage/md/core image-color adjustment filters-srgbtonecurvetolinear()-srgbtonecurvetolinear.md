

- Core Image
- Color Adjustment Filters
-  sRGBToneCurveToLinear() 

Type Method

# sRGBToneCurveToLinear()

Converts the colors in an image from sRGB to linear.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func sRGBToneCurveToLinear() -> any CIFilter & CISRGBToneCurveToLinear
```

## Return Value

The modified image.

## Discussion

This method applies the sRGB-tone-curve-to-linear filter to an image. The effect converts an image in sRGB space to linear color space.

The sRGB-tone-curve-to-linear filter uses the following properties:

`inputImage`  
An image with the type CIImage.

The following code creates a filter that converts from sRGB to linear color space.

func sRGBToLinear(inputImage: CIImage) -> CIImage {
    let sRGBToLinearFilter = CIFilter.sRGBToneCurveToLinear()
    sRGBToLinearFilter.inputImage = inputImage
    return sRGBToLinearFilter.outputImage!
}

## See Also

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

class func temperatureAndTint() -> any CIFilter &amp; CITemperatureAndTint

Alters an image’s temperature and tint.

class func toneCurve() -> any CIFilter &amp; CIToneCurve

Alters an image’s tone curve according to a series of data points.

class func vibrance() -> any CIFilter &amp; CIVibrance

Adjusts an image’s vibrancy.

class func whitePointAdjust() -> any CIFilter &amp; CIWhitePointAdjust

Adjusts the image’s white-point.

