

- Core Image
- Color Adjustment Filters
-  colorClamp() 

Type Method

# colorClamp()

Alters the colors in an image based on color components.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func colorClamp() -> any CIFilter & CIColorClamp
```

## Return Value

The modified image.

## Discussion

This method applies the color clamp filter to an image. The effect calculates each pixel’s color component value. Using this calculation, the effect adjusts the values that are outside the range of the `minComponents` or `maxComponents` properties and clamps them within the range.

The color clamp filter uses the following properties:

`minComponents`  
`RGBA` values for the lower end of the range as a CIVector.

`maxComponents`  
`RGBA` values for the upper end of the range as a `CIVector`.

`inputImage`  
An image with the type CIImage.

The following code creates a filter that adds a red hue to the input image:

func colorClamp(inputImage: CIImage) -> CIImage {
    let colorClampFilter = CIFilter.colorClamp()
    colorClampFilter.inputImage = inputImage
    colorClampFilter.minComponents = CIVector(x: 1, y: 0, z: 0, w: 0)
    colorClampFilter.maxComponents = CIVector (x: 1, y: 0.9, z: 1, w: 1)
    return colorClampFilter.outputImage!
}

## See Also

### Filters

class func colorAbsoluteDifference() -> any CIFilter &amp; CIColorAbsoluteDifference

Calculates the absolute difference between each color component in the input images.

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

