

- Core Image
- Stylizing Filters
-  cannyEdgeDetector() 

Type Method

# cannyEdgeDetector()

Applies the Canny edge-detection algorithm to an image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.5+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class func cannyEdgeDetector() -> any CIFilter & CICannyEdgeDetector
```

## Return Value

A CIImage with the detected edges.

## Discussion

This filter performs a Canny edge-detection on the input image, producing a black-and-white image with the detected edges. White pixels indicate an edge, and black pixels indicate no edge.

The Canny edge-detection filter uses the following properties:

`inputImage`  
The `CIImage` to use as an input for the effect.

`gaussianSigma`  
A `float` specifying the sigma of the Gaussian blur to apply, reducing high-frequency noise. Defaults to `1.6`.

`perceptual`  
A `Boolean` specifying whether to use a perceptual color space to compute the edge thresholds. Defaults to `false`.

`thresholdLow`  
A `float` specifying the threshold for weak edges. Defaults to `0.02`.

`thresholdHigh`  
A `float` specifying the threshold for strong edges. Defaults to `0.05`.

`hysteresisPasses`  
The number of hysteresis passes to apply to promote weak edge pixels. Minimum value is `0`, maximum value is `20`, and defaults to `1`.

The following code applies Canny edge-detection to an image:

func cannyEdgeDetector(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.cannyEdgeDetector()
    filter.inputImage = inputImage
    filter.gaussianSigma = 5
    filter.perceptual = false
    filter.thresholdLow = 0.02
    filter.thresholdHigh = 0.05
    filter.hysteresisPasses = 1
    return filter.outputImage!
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

class func lineOverlay() -> any CIFilter &amp; CILineOverlay

Creates an image that resembles a sketch of the outlines of objects.

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

