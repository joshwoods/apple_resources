

- Core Image
- Color Adjustment Filters
-  colorPolynomial() 

Type Method

# colorPolynomial()

Alters an image’s colors.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func colorPolynomial() -> any CIFilter & CIColorPolynomial
```

## Return Value

The modified image.

## Discussion

This method applies the color polynomial filter to an image. The effect calculates the sum of each pixel’s color component value and the coefficient properties together to produce the output image.

The color polynomial filter uses the following properties:

`redCoefficients`  
A vector representing the polynomial coefficients for the red channel as a CIVector.

`greenCoefficients`  
A vector representing the polynomial coefficients for the green channel as a `CIVector`.

`blueCoefficients`  
A vector representing the polynomial coefficients for the blue channel as a `CIVector`.

`alphaCoefficients`  
A vector representing the polynomial coefficients for the alpha channel as a `CIVector`.

`inputImage`  
An image with the type CIImage.

The following code creates a filter that adds a lighter contrast to the input image:

func colorPolynomial(inputImage: CIImage) -> CIImage {
    let colorPolynomialFilter = CIFilter.colorPolynomial()
    colorPolynomialFilter.alphaCoefficients = CIVector (x: 0, y: 0.6, z: 0, w: 0)
    colorPolynomialFilter.redCoefficients = CIVector (x: 0, y: 1, z: 0.1, w: 0)
    colorPolynomialFilter.greenCoefficients = CIVector(x: 0, y: 1, z: 0, w: 0)
    colorPolynomialFilter.blueCoefficients = CIVector(x: 0, y: 1, z: 0, w: 0)
    colorPolynomialFilter.inputImage = inputImage
    return colorPolynomialFilter.outputImage!
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

