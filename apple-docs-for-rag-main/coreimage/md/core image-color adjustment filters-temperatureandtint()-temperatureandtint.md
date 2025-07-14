

- Core Image
- Color Adjustment Filters
-  temperatureAndTint() 

Type Method

# temperatureAndTint()

Alters an image’s temperature and tint.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func temperatureAndTint() -> any CIFilter & CITemperatureAndTint
```

## Return Value

The modified image.

## Discussion

This method applies the image temperature and tint filter to an image. The effect adjusts the white balance of the input image to match the `targetNeutral` property, resulting in a cooler or warmer tone image.

The temperature and tint filter uses the following properties:

`neutral`  
A `vector` containing the source white point as a CIVector.

`targetNeutral`  
A vector containing the desired white point as a `CIVector`.

`inputImage`  
An image with the type CIImage.

The following code creates a filter that adds an orange hue to the input image:

func tempatureAndTint(inputImage: CIImage) -> CIImage {
    let tempatureAndTintFilter = CIFilter.temperatureAndTint()
    tempatureAndTintFilter.inputImage = inputImage
    tempatureAndTintFilter.neutral = CIVector(x: 11500, y: 10)
    tempatureAndTintFilter.targetNeutral = CIVector(x: 4000, y: 0)
    return tempatureAndTintFilter.outputImage!
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

class func sRGBToneCurveToLinear() -> any CIFilter &amp; CISRGBToneCurveToLinear

Converts the colors in an image from sRGB to linear.

class func toneCurve() -> any CIFilter &amp; CIToneCurve

Alters an image’s tone curve according to a series of data points.

class func vibrance() -> any CIFilter &amp; CIVibrance

Adjusts an image’s vibrancy.

class func whitePointAdjust() -> any CIFilter &amp; CIWhitePointAdjust

Adjusts the image’s white-point.

