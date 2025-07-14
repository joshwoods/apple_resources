

- Core Image
- Blur Filters
-  maskedVariableBlur() 

Type Method

# maskedVariableBlur()

Blurs a specified portion of an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func maskedVariableBlur() -> any CIFilter & CIMaskedVariableBlur
```

## Return Value

The blurred image.

## Discussion

This method applies the masked variable blur to an image. The effect blurs the image in an area defined by the mask image. The mask image contains shades of grey that define the strength of the blur. Black colors in the mask cause no blurring, and white colors cause maximum blur.

The masked variable blur filter uses the following properties:

`radius`  
A `float` representing the area of effect as an NSNumber.

`mask`  
An image that masks an area on the input image with the type CIImage.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that adds a blur to the bottom of the input image:

func maskedVariableBlur(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.maskedVariableBlur()
    filter.inputImage = inputImage
    // Create a mask that goes from white to black vertially.
    let mask = CIFilter.smoothLinearGradient()
    mask.color0 = CIColor.white
    mask.color1 = CIColor.black
    mask.point0 = CGPoint(x: 0, y: 0)
    mask.point1 = CGPoint(x:0, y: inputImage.extent.height)
    filter.mask = mask.outputImage
    filter.radius = 25
    return filter.outputImage!
}

## See Also

### Filters

class func bokehBlur() -> any CIFilter &amp; CIBokehBlur

Applies a bokeh effect to an image.

class func boxBlur() -> any CIFilter &amp; CIBoxBlur

Applies a square-shaped blur to an area of an image.

class func discBlur() -> any CIFilter &amp; CIDiscBlur

Applies a circle-shaped blur to an area of an image.

class func gaussianBlur() -> any CIFilter &amp; CIGaussianBlur

Blurs an image with a Gaussian distribution pattern.

class func median() -> any CIFilter &amp; CIMedian

Calculates the median of an image to refine detail.

class func morphologyGradient() -> any CIFilter &amp; CIMorphologyGradient

Detects and highlights edges of objects.

class func morphologyMaximum() -> any CIFilter &amp; CIMorphologyMaximum

Blurs a circular area by enlarging contrasting pixels.

class func morphologyMinimum() -> any CIFilter &amp; CIMorphologyMinimum

Blurs a circular area by reducing contrasting pixels.

class func morphologyRectangleMaximum() -> any CIFilter &amp; CIMorphologyRectangleMaximum

Blurs a rectangular area by enlarging contrasting pixels.

class func morphologyRectangleMinimum() -> any CIFilter &amp; CIMorphologyRectangleMinimum

Blurs a rectangular area by reducing contrasting pixels.

class func motionBlur() -> any CIFilter &amp; CIMotionBlur

Creates motion blur on an image.

class func noiseReduction() -> any CIFilter &amp; CINoiseReduction

Reduces noise by sharpening the edges of objects.

class func zoomBlur() -> any CIFilter &amp; CIZoomBlur

Creates a zoom blur centered around a single point on the image.

