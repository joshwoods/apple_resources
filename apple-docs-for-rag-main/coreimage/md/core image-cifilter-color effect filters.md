

- Core Image
- CIFilter
-  Color Effect Filters 

API Collection

# Color Effect Filters

## Topics

### Filters

class func colorCrossPolynomial() -> any CIFilter &amp; CIColorCrossPolynomial

Adjusts an image’s color by applying polynomial cross-products.

class func colorCube() -> any CIFilter &amp; CIColorCube

Adjusts an image’s pixels using a three-dimensional color table.

class func colorCubeWithColorSpace() -> any CIFilter &amp; CIColorCubeWithColorSpace

Adjusts an image’s pixels using a three-dimensional color table in specified color space.

class func colorCubesMixedWithMask() -> any CIFilter &amp; CIColorCubesMixedWithMask

Alters an image’s pixels using a three-dimensional color tables and a mask image.

class func colorCurves() -> any CIFilter &amp; CIColorCurves

Adjusts an image’s color curves.

class func colorInvert() -> any CIFilter &amp; CIColorInvert

Inverts an image’s colors.

class func colorMap() -> any CIFilter &amp; CIColorMap

Performs a transformation of the input image colors to colors from a gradient image.

class func colorMonochrome() -> any CIFilter &amp; CIColorMonochrome

Adjusts an image’s colors to shades of a single color.

class func colorPosterize() -> any CIFilter &amp; CIColorPosterize

Flattens an image’s colors.

class func convertLabToRGB() -> any CIFilter &amp; CIConvertLab

Converts an image from CIELAB to RGB color space.

class func convertRGBtoLab() -> any CIFilter &amp; CIConvertLab

Converts an image from RGB to CIELAB color space.

class func dither() -> any CIFilter &amp; CIDither

Applies randomized noise to produce a processed look.

class func documentEnhancer() -> any CIFilter &amp; CIDocumentEnhancer

Adjusts an image’s shadows and contrast.

class func falseColor() -> any CIFilter &amp; CIFalseColor

Replaces an image’s colors with specified colors.

class func labDeltaE() -> any CIFilter &amp; CILabDeltaE

Compares an image’s color values.

class func maskToAlpha() -> any CIFilter &amp; CIMaskToAlpha

Converts an image to a white image with an alpha component.

class func maximumComponent() -> any CIFilter &amp; CIMaximumComponent

Creates a maximum RGB grayscale image.

class func minimumComponent() -> any CIFilter &amp; CIMinimumComponent

Creates a minimum RGB grayscale image.

class func paletteCentroid() -> any CIFilter &amp; CIPaletteCentroid

Calculates the location of an image’s colors.

class func palettize() -> any CIFilter &amp; CIPalettize

Replaces colors with colors from a palette image.

class func photoEffectChrome() -> any CIFilter &amp; CIPhotoEffect

Exaggerates an image’s colors.

class func photoEffectFade() -> any CIFilter &amp; CIPhotoEffect

Diminishes an image’s colors.

class func photoEffectInstant() -> any CIFilter &amp; CIPhotoEffect

Desaturates an image’s colors.

class func photoEffectMono() -> any CIFilter &amp; CIPhotoEffect

Adjust an image’s colors to black and white.

class func photoEffectNoir() -> any CIFilter &amp; CIPhotoEffect

Adjusts an image’s colors to black and white and intensifies the contrast.

class func photoEffectProcess() -> any CIFilter &amp; CIPhotoEffect

Lowers the contrast of the input image.

class func photoEffectTonal() -> any CIFilter &amp; CIPhotoEffect

Adjusts an image’s colors to black and white.

class func photoEffectTransfer() -> any CIFilter &amp; CIPhotoEffect

Brightens an image’s colors.

class func sepiaTone() -> any CIFilter &amp; CISepiaTone

Adjusts an image’s colors to shades of brown.

class func thermal() -> any CIFilter &amp; CIThermal

Alters the image to make it look like it was taken by a thermal camera.

class func vignetteEffect() -> any CIFilter &amp; CIVignetteEffect

Gradually darkens a specified area of an image.

class func vignette() -> any CIFilter &amp; CIVignette

Gradually darkens an image’s edges.

class func xRay() -> any CIFilter &amp; CIXRay

Alters an image to make it look like an X-ray image.

### Protocols

protocol CIColorCrossPolynomial

The properties you use to configure a color cross-polynomial filter.

protocol CIColorCube

The properties you use to configure a color cube filter.

protocol CIColorCubeWithColorSpace

The properties you use to configure a color cube with color space filter.

protocol CIColorCubesMixedWithMask

The properties you use to configure a color cube mixed with mask filter.

protocol CIColorCurves

The properties you use to configure a color curves filter.

protocol CIColorInvert

The properties you use to configure a color invert filter.

protocol CIColorMap

The properties you use to configure a color map filter.

protocol CIColorMonochrome

The properties you use to configure a color monochrome filter.

protocol CIConvertLab

protocol CIDither

The properties you use to configure a dither filter.

protocol CIColorPosterize

The properties you use to configure a color posterize filter.

protocol CIDocumentEnhancer

The properties you use to configure a document enhancer filter.

protocol CIFalseColor

The properties you use to configure a false color filter.

protocol CILabDeltaE

The properties you use to configure a Lab Delta E filter.

protocol CIMaskToAlpha

The properties you use to configure a mask-to-alpha filter.

protocol CIMaximumComponent

The properties you use to configure a maximum component filter.

protocol CIMinimumComponent

The properties you use to configure a minimum component filter.

protocol CIPaletteCentroid

The properties you use to configure a palette centroid filter.

protocol CIPalettize

The properties you use to configure a palettize filter.

protocol CIPhotoEffect

The properties you use to configure a photo-effect filter.

protocol CISepiaTone

The properties you use to configure a sepia-tone filter.

protocol CIThermal

The properties you use to configure a thermal filter.

protocol CIVignette

The properties you use to configure a vignette filter.

protocol CIVignetteEffect

The properties you use to configure a vignette-effect filter.

protocol CIXRay

The properties you use to configure an X-ray filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Adjustment Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

