

- Core Image
- Gradient Filters
-  hueSaturationValueGradient() 

Type Method

# hueSaturationValueGradient()

Generates a gradient representing a specified color space.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func hueSaturationValueGradient() -> any CIFilter & CIHueSaturationValueGradient
```

## Return Value

The generated image.

## Discussion

This method generates a hue-saturation-value gradient image. The filter creates a color wheel that shows the hues and saturations for a specified CGColorSpace.

The hue-saturation-value gradient uses the following properties:

`colorSpace`  
A `CGColorSpace` representing the color space for the generated color wheel.

`dither`  
A `boolean` value specifying whether the distort the generated output.

`radius`  
A `float` representing the distance from the center of the effect as an NSNumber.

`softness`  
A `float` representing the softness of the generated color wheel as an `NSNumber`.

`value`  
A `float` representing the lightness of the hue-saturation gradient as an `NSNumber`.

The following code creates a filter that generates a color-space image:

func hueSaturationValue() -> CIImage {
    let hueSaturationValueGradient = CIFilter.hueSaturationValueGradient()
    hueSaturationValueGradient.colorSpace = CGColorSpaceCreateDeviceRGB()
    hueSaturationValueGradient.dither = 1
    hueSaturationValueGradient.radius = 100
    hueSaturationValueGradient.softness = 2
    hueSaturationValueGradient.value = 1
    return hueSaturationValueGradient.outputImage!
}

## See Also

### Filters

class func gaussianGradient() -> any CIFilter &amp; CIGaussianGradient

Generates a gradient that varies from one color to another using a Gaussian distribution.

class func linearGradient() -> any CIFilter &amp; CILinearGradient

Generates a color gradient that varies along a linear axis between two defined endpoints.

class func radialGradient() -> any CIFilter &amp; CIRadialGradient

Generates a gradient that varies radially between two circles having the same center.

class func smoothLinearGradient() -> any CIFilter &amp; CISmoothLinearGradient

Generates a gradient that blends colors along a linear axis between two defined endpoints.

