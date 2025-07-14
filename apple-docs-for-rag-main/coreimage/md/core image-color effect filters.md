

- Core Image
-  Color Effect Filters 

API Collection

# Color Effect Filters

Apply color effects, including photo effects, dithering, and color maps.

## Topics

### Color Effect Filters

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

class func vignette() -> any CIFilter &amp; CIVignette

Gradually darkens an image’s edges.

class func vignetteEffect() -> any CIFilter &amp; CIVignetteEffect

Gradually darkens a specified area of an image.

class func xRay() -> any CIFilter &amp; CIXRay

Alters an image to make it look like an X-ray image.

## See Also

### Filter Catalog

Blur Filters

Apply blurs, simulate motion and zoom effects, reduce noise, and erode and dilate image regions.

Color Adjustment Filters

Apply color transformations, including exposure, hue, and tint adjustments.

Composite Operations

Composite images by using a range of blend modes and compositing operators.

Convolution Filters

Produce effects such as blurring, sharpening, edge detection, translation, and embossing.

Distortion Filters

Apply distortion to images.

Generator Filters

Generate barcode, geometric, and special-effect images.

Geometry Adjustment Filters

Translate, scale, and rotate images in 2D and 3D.

Gradient Filters

Generate linear and radial gradients.

Halftone Effect Filters

Simulate monochrome and CMYK halftone screens.

Reduction Filters

Create statistical information about an image.

Sharpening Filters

Apply sharpening to images.

Stylizing Filters

Create stylized versions of images by applying effects including pixelation and line overlays.

Tile Effect Filters

Produce tiled images from source images.

Transition Filters

Transition between two images by using effects including page curl and swipe.

