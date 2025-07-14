

- Core Image
- Stylizing Filters
-  lineOverlay() 

Type Method

# lineOverlay()

Creates an image that resembles a sketch of the outlines of objects.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func lineOverlay() -> any CIFilter & CILineOverlay
```

## Return Value

The modified image.

## Discussion

This method applies the line overlay filter to an image. The effect creats a sketch that outlines the edges of the image in black, leaving the non-outlined portion of the image transparent.

The line overlay filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`nrNoiseLevel`  
A `float` representing the desired level of noise as an NSNumber.

`nrSharpness`  
A `float` representing the desired level of sharpness as an `NSNumber`.

`edgeIntensity`  
A `float` representing the Sobel gradient information for edge tracing as an `NSNumber`.

`threshold`  
A `float` representing the threshold of edge visibilty as an `NSNumber`.

`contrast`  
A `float` representing the desired contrast as an `NSNumber`.

The following code creates a filter that results in a monochrome image with lines outlining the edges of objects:

func lineOverlay(inputImage: CIImage) -> CIImage {
    let lineOverlay = CIFilter.lineOverlay()
    lineOverlay.inputImage = inputImage
    lineOverlay.nrNoiseLevel = 0.07
    lineOverlay.nrSharpness = 0.71
    lineOverlay.edgeIntensity = 1
    lineOverlay.threshold = 0.1
    lineOverlay.contrast = 50.00
    return lineOverlay.outputImage!
}

## See Also

### Filters

class func blendWithAlphaMask() -> any CIFilter &amp; CIBlendWithMask

Blends two images by using an alpha mask image.

class func blendWithBlueMask() -> any CIFilter &amp; CIBlendWithMask

Blends two images by using a blue mask image.

class func blendWithMask() -> any CIFilter &amp; CIBlendWithMask

Blends two images by using a mask image.

class func blendWithRedMask() -> any CIFilter &amp; CIBlendWithMask

Blends two images by using a red mask image.

class func bloom() -> any CIFilter &amp; CIBloom

Adjusts an image’s colors by applying a blur effect.

class func comicEffect() -> any CIFilter &amp; CIComicEffect

Creates an image with a comic book effect.

class func coreMLModel() -> any CIFilter &amp; CICoreMLModel

Filters an image with a Core ML model.

class func crystallize() -> any CIFilter &amp; CICrystallize

Creates an image made with a series of colorful polygons.

class func depthOfField() -> any CIFilter &amp; CIDepthOfField

Simulates a depth of field effect.

class func edges() -> any CIFilter &amp; CIEdges

Hilghlights edges of objects found within an image.

class func edgeWork() -> any CIFilter &amp; CIEdgeWork

Produces a black-and-white image that looks similar to a woodblock print.

class func gaborGradients() -> any CIFilter &amp; CIGaborGradients

Highlights textures in an image.

class func gloom() -> any CIFilter &amp; CIGloom

Adjusts an image’s color by applying a gloom filter.

class func heightFieldFromMask() -> any CIFilter &amp; CIHeightFieldFromMask

Creates a realistic shaded height-field image.

class func hexagonalPixellate() -> any CIFilter &amp; CIHexagonalPixellate

Creates an image made of a series of colorful hexagons.

class func highlightShadowAdjust() -> any CIFilter &amp; CIHighlightShadowAdjust

Adjusts the highlights of colors to reduce shadows.

class func mix() -> any CIFilter &amp; CIMix

Blends two images together.

class func personSegmentation() -> any CIFilter &amp; CIPersonSegmentation

Creates a mask where red pixels indicate areas of the image that are likely to contain a person.

class func pixellate() -> any CIFilter &amp; CIPixellate

Enlarges the colors of the pixels to create a blurred effect.

class func pointillize() -> any CIFilter &amp; CIPointillize

Applies a pointillize effect to an image.

class func saliencyMap() -> any CIFilter &amp; CISaliencyMap

Creates a saliency map from an image.

class func shadedMaterial() -> any CIFilter &amp; CIShadedMaterial

Creates a shaded image from a height-field image.

class func sobelGradients() -> any CIFilter &amp; CISobelGradients

Calculates the Sobel gradients for an image.

class func spotColor() -> any CIFilter &amp; CISpotColor

Replaces colors of an image with specifed colors.

class func spotLight() -> any CIFilter &amp; CISpotLight

Highlights a definined area of the image.

class func cannyEdgeDetector() -> any CIFilter &amp; CICannyEdgeDetector

Applies the Canny edge-detection algorithm to an image.

