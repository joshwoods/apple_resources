

- Core Image
- Stylizing Filters
-  spotColor() 

Type Method

# spotColor()

Replaces colors of an image with specifed colors.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func spotColor() -> any CIFilter & CISpotColor
```

## Return Value

The modified image.

## Discussion

This method applies the spot color filter to an image. The effect replaces one or more of the color ranges of the input image with properties.

The spot color filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`centerColor1`  
A CIColor representing the median value of the first color to be replaced.

`centerColor2`  
A `CIColor` representing the median value of the second color to be replaced.

`centerColor3`  
A `CIColor` representing the median value of the third color to be replaced.

`replacementColor1`  
A `CIColor` to replace the first color.

`replacementColor2`  
A `CIColor` to replace the second color.

`replacementColor3`  
A `CIColor` to replace the third color.

`closeness1`  
A `float` representing how closely the first center color must match before it’s replaced.

`closeness2`  
A `float` representing how closely the second center color must match before it’s replaced.

`closeness3`  
A `float` representing how closely the third center color must match before it’s replaced.

`contrast1`  
A `float` representing the contrast of the first replacement color as an NSNumber.

`contrast2`  
A `float` representing the contrast of the second replacement color as an `NSNumber`.

`contrast3`  
A `float` representing the contrast of the third replacement color as an `NSNumber`.

The following code creates a filter that replaces the colors of the input image with the specified colors:

func spotColor(inputImage: CIImage) -> CIImage {
    let spotColorFilter = CIFilter.spotColor()
    spotColorFilter.inputImage = inputImage
    spotColorFilter.centerColor1 = .red
    spotColorFilter.replacementColor1 = .green
    spotColorFilter.closeness1 = 5
    spotColorFilter.contrast1 = 1
    return spotColorFilter.outputImage!
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

class func spotLight() -> any CIFilter &amp; CISpotLight

Highlights a definined area of the image.

class func cannyEdgeDetector() -> any CIFilter &amp; CICannyEdgeDetector

Applies the Canny edge-detection algorithm to an image.

