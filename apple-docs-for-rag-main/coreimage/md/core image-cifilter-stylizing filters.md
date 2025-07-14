

- Core Image
- CIFilter
-  Stylizing Filters 

API Collection

# Stylizing Filters

## Topics

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

class func cannyEdgeDetector() -> any CIFilter &amp; CICannyEdgeDetector

Applies the Canny edge-detection algorithm to an image.

class func comicEffect() -> any CIFilter &amp; CIComicEffect

Creates an image with a comic book effect.

class func coreMLModel() -> any CIFilter &amp; CICoreMLModel

Filters an image with a Core ML model.

class func crystallize() -> any CIFilter &amp; CICrystallize

Creates an image made with a series of colorful polygons.

class func depthOfField() -> any CIFilter &amp; CIDepthOfField

Simulates a depth of field effect.

class func edgeWork() -> any CIFilter &amp; CIEdgeWork

Produces a black-and-white image that looks similar to a woodblock print.

class func edges() -> any CIFilter &amp; CIEdges

Hilghlights edges of objects found within an image.

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

### Protocols

protocol CIBlendWithMask

The properties you use to configure a blend with mask filter.

protocol CIBloom

The properties you use to configure a bloom filter.

protocol CICannyEdgeDetector

protocol CIComicEffect

The properties you use to configure a comic effect filter.

protocol CICoreMLModel

The properties you use to configure a Core ML model filter.

protocol CICrystallize

The properties you use to configure a crystalize filter.

protocol CIDepthOfField

The properties you use to configure a depth-of-field filter.

protocol CIEdgeWork

The properties you use to configure an edge-work filter.

protocol CIEdges

The properties you use to configure an edges filter.

protocol CIGaborGradients

protocol CIGloom

The properties you use to configure a gloom filter.

protocol CIHeightFieldFromMask

The properties you use to configure a height-field-from-mask filter.

protocol CIHexagonalPixellate

The properties you use to configure a hexagonal pixellate filter.

protocol CIHighlightShadowAdjust

The properties you use to configure a highlight-shadow adjust filter.

protocol CILineOverlay

The properties you use to configure a line overlay filter.

protocol CIMix

The properties you use to configure a mix filter.

protocol CIPersonSegmentation

protocol CIPixellate

The properties you use to configure a pixellate filter.

protocol CIPointillize

The properties you use to configure a pointillize filter.

protocol CISaliencyMap

The properties you use to configure a saliency map filter.

protocol CIShadedMaterial

The properties you use to configure a shaded material filter.

protocol CISobelGradients

protocol CISpotColor

The properties you use to configure a spot color filter.

protocol CISpotLight

The properties you use to configure a spotlight filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Tile Effect Filters

Transition Filters

