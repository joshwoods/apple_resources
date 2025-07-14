

- Core Image
- Gradient Filters
-  gaussianGradient() 

Type Method

# gaussianGradient()

Generates a gradient that varies from one color to another using a Gaussian distribution.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func gaussianGradient() -> any CIFilter & CIGaussianGradient
```

## Return Value

The generated image.

## Discussion

This method generates a Gaussian gradient image. The effect uses the Gaussian kernel to calculate the even dispersal of the first color in the center to the second color in the image’s periphery.

The Gaussian gradient filter uses the following properties:

`center`  
A CGPoint representing the center of the effect as x and y coordinates.

`color0`  
A CIColor representing the first color to use in the gradient.

`color1`  
A `CIColor` representing the second color to use in the gradient.

`radius`  
A `float` representing the radius of the Gaussian distribution as an NSNumber.

The following code creates a filter that generates a gradient image:

func gaussian() -> CIImage {
    let gaussianGradient = CIFilter.gaussianGradient()
    gaussianGradient.center = CGPoint (x: 150, y: 150)
    gaussianGradient.color0 = CIColor(red: 88/255, green: 201
/255, blue: 175/255)
    gaussianGradient.color1 = CIColor(red: 153/255, green: 153/255, blue: 204/255)
    gaussianGradient.radius = 10
    return gaussianGradient.outputImage!
}

## See Also

### Filters

class func hueSaturationValueGradient() -> any CIFilter &amp; CIHueSaturationValueGradient

Generates a gradient representing a specified color space.

class func linearGradient() -> any CIFilter &amp; CILinearGradient

Generates a color gradient that varies along a linear axis between two defined endpoints.

class func radialGradient() -> any CIFilter &amp; CIRadialGradient

Generates a gradient that varies radially between two circles having the same center.

class func smoothLinearGradient() -> any CIFilter &amp; CISmoothLinearGradient

Generates a gradient that blends colors along a linear axis between two defined endpoints.

