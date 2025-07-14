

- Core Image
- Blur Filters
-  morphologyRectangleMinimum() 

Type Method

# morphologyRectangleMinimum()

Blurs a rectangular area by reducing contrasting pixels.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func morphologyRectangleMinimum() -> any CIFilter & CIMorphologyRectangleMinimum
```

## Return Value

The blurred image.

## Discussion

This method applies the morphology rectangle minimum filter to an image. The effect targets a rectangular section of the image, calculating the median color values to find colors that make up more than half the working area. Using this calculation, the effect reduces the pixels with contrasting colors to take up more of the less area. The effect is then repeated throughout the image.

The morphology rectangle minimum filter uses the following properties:

width  
A `float` representing the width in pixels of the working area as an NSNumber.

height  
A `float` representing the height in pixels of the working area as an NSNumber.

inputImage  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that adds an intense blur to the palm trees input image:

    func morphologyRectangleMinimum(inputImage: CIImage) -> CIImage? {

        let morphologyRectangleMinimumFilter = CIFilter.morphologyRectangleMinimum()
        morphologyRectangleMinimumFilter.inputImage = inputImage
        morphologyRectangleMinimumFilter.width = 5
        morphologyRectangleMinimumFilter.height = 5
        return morphologyRectangleMinimumFilter.outputImage
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

class func motionBlur() -> any CIFilter &amp; CIMotionBlur

Creates motion blur on an image.

class func noiseReduction() -> any CIFilter &amp; CINoiseReduction

Reduces noise by sharpening the edges of objects.

class func zoomBlur() -> any CIFilter &amp; CIZoomBlur

Creates a zoom blur centered around a single point on the image.

