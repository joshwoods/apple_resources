

- Core Image
- Blur Filters
-  noiseReduction() 

Type Method

# noiseReduction()

Reduces noise by sharpening the edges of objects.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func noiseReduction() -> any CIFilter & CINoiseReduction
```

## Return Value

The blurred image.

## Discussion

This method applies the noise reduction filter to an image. The effect calculates changes in luminance below the noise level and locally blurs the area. Values above the threshold are determined to be edges, and become sharpened.

The morphology noise reduction filter uses the following properties:

`noiseLevel`  
A `float` representing the amount of noise reduction as an NSNumber.

`sharpness`  
A `float` representing the sharpness of the final image as an NSNumber.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that reduces noise in the input image:

    func noiseReduction(inputImage: CIImage) -> CIImage? {

        let noiseReductionfilter = CIFilter.noiseReduction()
        noiseReductionfilter.inputImage = inputImage
        noiseReductionfilter.noiseLevel = 0.2
        noiseReductionfilter.sharpness = 0.4
        return noiseReductionfilter.outputImage
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

class func zoomBlur() -> any CIFilter &amp; CIZoomBlur

Creates a zoom blur centered around a single point on the image.

