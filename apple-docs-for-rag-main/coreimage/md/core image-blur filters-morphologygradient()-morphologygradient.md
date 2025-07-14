

- Core Image
- Blur Filters
-  morphologyGradient() 

Type Method

# morphologyGradient()

Detects and highlights edges of objects.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func morphologyGradient() -> any CIFilter & CIMorphologyGradient
```

## Return Value

The blurred image.

## Discussion

This method applies the morphology gradient filter to an image. The effect uses the `radius` to compute and highlight edges of items within the image.

The morphology gradient filter uses the following properties:

`radius`  
A `float` representing the area of effect as an NSNumber.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that adds darkness to the overall image while the edges in the input photo become brighter:

    func morphologyGradient(inputImage: CIImage) -> CIImage? {

        let morphologyGradientFilter = CIFilter.morphologyGradient()
        morphologyGradientFilter.inputImage = inputImage
        morphologyGradientFilter.radius = 1
        return morphologyGradientFilter.outputImage
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

