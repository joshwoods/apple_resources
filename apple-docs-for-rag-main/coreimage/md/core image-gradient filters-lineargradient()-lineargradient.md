

- Core Image
- Gradient Filters
-  linearGradient() 

Type Method

# linearGradient()

Generates a color gradient that varies along a linear axis between two defined endpoints.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func linearGradient() -> any CIFilter & CILinearGradient
```

## Return Value

The generated image.

## Discussion

This method generates a linear-gradient image. The effect creates a gradient that varies linearly between the two input properties of `point0` and `point1`.

The linear-gradient filter uses the following properties:

`point0`  
A CGPoint representing the starting position of the gradient.

`point1`  
A `CGPoint` representing the ending position of the gradient.

`color0`  
A CIColor representing the first color to use in the gradient.

`color1`  
A `CIColor` representing the second color to use the gradient.

The following code creates a filter that generates a gradient image:

func linear() -> CIImage {
    let linearGradient = CIFilter.linearGradient()
    linearGradient.point0 = CGPoint(x: 0, y: 0)
    linearGradient.point1 = CGPoint(x: 200, y: 200)
    linearGradient.color0 = CIColor(red: 216/255, green: 232/255, blue: 146/255)
    linearGradient.color1 = CIColor(red: 0/255, green: 112/255, blue: 201/255)
    return linearGradient.outputImage!
}

## See Also

### Filters

class func gaussianGradient() -> any CIFilter &amp; CIGaussianGradient

Generates a gradient that varies from one color to another using a Gaussian distribution.

class func hueSaturationValueGradient() -> any CIFilter &amp; CIHueSaturationValueGradient

Generates a gradient representing a specified color space.

class func radialGradient() -> any CIFilter &amp; CIRadialGradient

Generates a gradient that varies radially between two circles having the same center.

class func smoothLinearGradient() -> any CIFilter &amp; CISmoothLinearGradient

Generates a gradient that blends colors along a linear axis between two defined endpoints.

