

- Core Image
- Blur Filters
-  zoomBlur() 

Type Method

# zoomBlur()

Creates a zoom blur centered around a single point on the image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func zoomBlur() -> any CIFilter & CIZoomBlur
```

## Return Value

The blurred image.

## Discussion

This method applies the zoom blur filter to an image. This effect mimics the zoom of a camera when capturing the image.

The zoom blur filter uses the following properties:

`amount`  
A `float` representing the zoom-in amount as an NSNumber.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that adds a zoom blur to the input image:

    func zoomBlur(inputImage: CIImage) -> CIImage? {

        let zoomBlurFilter = CIFilter.zoomBlur()
        zoomBlurFilter.inputImage = inputImage
        zoomBlurFilter.amount = 5
        zoomBlurFilter.center = CGPoint(x: 150, y: 150)
        return zoomBlurFilter.outputImage
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

