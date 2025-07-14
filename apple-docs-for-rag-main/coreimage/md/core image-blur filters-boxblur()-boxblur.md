

- Core Image
- Blur Filters
-  boxBlur() 

Type Method

# boxBlur()

Applies a square-shaped blur to an area of an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func boxBlur() -> any CIFilter & CIBoxBlur
```

## Return Value

The blurred image.

## Discussion

This method applies the box blur filter to an image. The effect targets a square area and calculates the median color value of the pixels to create the output image. The `radius` is the width of a square area with a larger area, resulting in a stronger blur effect on the output image.

The box blur filter uses the following properties:

`radius`  
A `float` representing the area of effect as a NSNumber.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that results in less detail in the input image:

    func boxBlur(inputImage: CIImage) -> CIImage? {

        let boxBlurFilter = CIFilter.boxBlur()
        boxBlurFilter.inputImage = inputImage
        boxBlurFilter.radius = 10
        return boxBlurFilter.outputImage
    }

## See Also

### Filters

class func bokehBlur() -> any CIFilter &amp; CIBokehBlur

Applies a bokeh effect to an image.

class func discBlur() -> any CIFilter &amp; CIDiscBlur

Applies a circle-shaped blur to an area of an image.

class func gaussianBlur() -> any CIFilter &amp; CIGaussianBlur

Blurs an image with a Gaussian distribution pattern.

class func maskedVariableBlur() -> any CIFilter &amp; CIMaskedVariableBlur

Blurs a specified portion of an image.

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

