

- Core Image
- Color Adjustment Filters
-  toneCurve() 

Type Method

# toneCurve()

Alters an image’s tone curve according to a series of data points.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func toneCurve() -> any CIFilter & CIToneCurve
```

## Return Value

The modified image.

## Discussion

This method applies the tone curve filter to an image. The effect calculates the adjustment of the tone curve by the sum of the red, green, and blue color values with the point value properties specified.

The tone curve filter uses the following properties:

`point0`  
A v`ector` containing the position of the first point of the tone curve as a CIVector.

`point1`  
A v`ector` containing the position of the second point of the tone curve as a `CIVector`.

`point2`  
A `vector` containing the position of the third point of the tone curve as a `CIVector`.

`point3`  
A v`ector` containing the position of the fourth point of the tone curve as a `CIVector`.

`point4`  
A v`ector` containing the position of the fifth point of the tone curve as a `CIVector`.

`inputImage`  
An image with the type CIImage.

The following code creates a filter that adds brightness to the input image:

func toneCurve(inputImage: CIImage) -> CIImage {
    let toneCurveFilter = CIFilter.toneCurve()
    toneCurveFilter.inputImage = inputImage
    toneCurveFilter.point0 = CGPoint(x: 0, y: 0)
    toneCurveFilter.point1 = CGPoint(x: 0.22, y: 0.25)
    toneCurveFilter.point2 = CGPoint(x: 0.4, y: 0.5)
    toneCurveFilter.point3 = CGPoint(x: 0.65, y: 0.75)
    toneCurveFilter.point4 = CGPoint(x: 1, y: 1)
    return toneCurveFilter.outputImage!
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

class func temperatureAndTint() -> any CIFilter &amp; CITemperatureAndTint

Alters an image’s temperature and tint.

class func vibrance() -> any CIFilter &amp; CIVibrance

Adjusts an image’s vibrancy.

class func whitePointAdjust() -> any CIFilter &amp; CIWhitePointAdjust

Adjusts the image’s white-point.

