

- Core Image
- Stylizing Filters
-  coreMLModel() 

Type Method

# coreMLModel()

Filters an image with a Core ML model.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func coreMLModel() -> any CIFilter & CICoreMLModel
```

## Return Value

The modified image.

## Discussion

This method applies the Core ML model filter to an image. The effect filters the image using a trained Core ML model to produce the result. Specifying the head index allows you to produce a result from various components of a multiheaded coreML model.

The Core ML model filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`headIndex`  
A `float` representing which output of a multihead Core ML model should be used for applying the effect to an image.

`softmaxNormalization`  
A `Boolean` value representing the softmax normalization to be applied to the output image created by the model.

`inputModel`  
The Core ML model to be used for applying effect on the image.

The following code creates a filter that results in the flowers appearing to be glass panes:

func coreML(inputImage: CIImage) -> CIImage {
    let coreMLFilter = CIFilter.coreMLModel()
    let model = GlassModel().model
    coreMLFilter.inputImage = inputImage
    coreMLFilter.headIndex = 0
    coreMLFilter.softmaxNormalization = false
    return coreMLFilter.outputImage!
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

class func cannyEdgeDetector() -> any CIFilter &amp; CICannyEdgeDetector

Applies the Canny edge-detection algorithm to an image.

