

- Core Image
- Blur Filters
-  morphologyMaximum() 

Type Method

# morphologyMaximum()

Blurs a circular area by enlarging contrasting pixels.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func morphologyMaximum() -> any CIFilter & CIMorphologyMaximum
```

## Return Value

The blurred image.

## Discussion

This method applies the morphology maximum filter to an image. The effect targets a circular section of the image, calculating the median color values to find colors that make up more than half the working area. Using this calculation, the effect enlarges the pixels with contrasting colors to take up more of the working area. The effect is then repeated throughout the image.

The morphology maximum filter uses the following properties:

`radius`  
A `float` representing the area of effect as an NSNumber.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that adds an intense blur to the input image:

    func morphologyMaximum(inputImage: CIImage) -> CIImage? {

        let morphologyMaximumFilter = CIFilter.morphologyMaximum()
        morphologyMaximumFilter.inputImage = inputImage
        morphologyMaximumFilter.radius = 5
        return morphologyMaximumFilter.outputImage
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

