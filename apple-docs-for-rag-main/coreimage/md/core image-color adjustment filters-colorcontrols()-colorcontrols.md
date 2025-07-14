

- Core Image
- Color Adjustment Filters
-  colorControls() 

Type Method

# colorControls()

Alters the brightness, contrast, and saturation of an image’s colors.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func colorControls() -> any CIFilter & CIColorControls
```

## Return Value

The modified image.

## Discussion

This method applies the color controls filter to an image. The effect calculates saturation by linearly interpolating between a grayscale image with a saturation of `0.0` and the original image saturation of `1.0.`

The color controls filter uses the following properties:

`brightness`  
A `float` representing the amount of brightness applied as a NSNumber.

`contrast`  
A `float` `r`epresenting the amount of contrast applied as a NSNumber.

`saturation`  
A float representing the amount of saturation applied as a NSNumber.

`inputImage`  
An image with the type CIImage.

The following code creates a filter that results in a darker image:

func colorControls(inputImage: CIImage) -> CIImage {
    let colorControlsFilter = CIFilter.colorControls()
    colorControlsFilter.inputImage = inputImage
    colorControlsFilter.brightness = -0.4
    colorControlsFilter.contrast = 1
    colorControlsFilter.saturation = 1
    return colorControlsFilter.outputImage!
}

## See Also

### Filters

class func colorAbsoluteDifference() -> any CIFilter &amp; CIColorAbsoluteDifference

Calculates the absolute difference between each color component in the input images.

class func colorClamp() -> any CIFilter &amp; CIColorClamp

Alters the colors in an image based on color components.

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

