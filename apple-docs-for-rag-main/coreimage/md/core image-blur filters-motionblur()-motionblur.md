

- Core Image
- Blur Filters
-  motionBlur() 

Type Method

# motionBlur()

Creates motion blur on an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func motionBlur() -> any CIFilter & CIMotionBlur
```

## Return Value

The blurred image.

## Discussion

This method applies the motion blur filter to an image. The filter uses the angle of a single row of pixels to determine the direction of the motion effect.

The motion blur filter uses the following properties:

`radius`  
A `float` representing the area of effect as an NSNumber.

`angle`  
A `float` representing the angle of the motion, in radians, that determines which direction the blur smears as an NSNumber.

`inputImage`  
A CIImage representing the input image to apply the filter to.

The following code creates a filter that adds a motion blur to the input image:

    func motionBlur(inputImage: CIImage) -> CIImage? {

        let motionBlurFilter = CIFilter.motionBlur()
        motionBlurFilter.inputImage = inputImage
        motionBlurFilter.angle = 0
        motionBlurFilter.radius = 20
        return motionBlurFilter.outputImage
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

class func noiseReduction() -> any CIFilter &amp; CINoiseReduction

Reduces noise by sharpening the edges of objects.

class func zoomBlur() -> any CIFilter &amp; CIZoomBlur

Creates a zoom blur centered around a single point on the image.

