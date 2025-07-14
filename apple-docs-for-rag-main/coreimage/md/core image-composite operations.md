

- Core Image
-  Composite Operations 

API Collection

# Composite Operations

Composite images by using a range of blend modes and compositing operators.

## Topics

### Filters

class func additionCompositing() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by addition.

class func colorBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images using the luminance values from the background image and the hue and saturation values from the input image.

class func colorBurnBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images while darkening the image.

class func colorDodgeBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images using dodging.

class func darkenBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images while darkening lighter pixels.

class func differenceBlendMode() -> any CIFilter &amp; CICompositeOperation

Subtracts color values to blend colors.

class func divideBlendMode() -> any CIFilter &amp; CICompositeOperation

Divides color values to blend colors.

class func exclusionBlendMode() -> any CIFilter &amp; CICompositeOperation

Subtracts color values to blend colors with less contrast.

class func hardLightBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by screening and multiplying.

class func hueBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by computing the sum of image color values.

class func lightenBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by brightening colors.

class func linearBurnBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images while increasing contrast.

class func linearDodgeBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images with dodging.

class func linearLightBlendMode() -> any CIFilter &amp; CICompositeOperation

A combination of linear burn and linear dodge blend modes.

class func luminosityBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends color from two images by calculating the color, hue, and saturation.

class func minimumCompositing() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by computing minimum values.

class func maximumCompositing() -> any CIFilter &amp; CICompositeOperation

Applies a maximum compositing filter to an image.

class func multiplyBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors from two images by multiplying color components.

class func multiplyCompositing() -> any CIFilter &amp; CICompositeOperation

Blurs the colors of two images by multiplying color components.

class func overlayBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors by overlaying images.

class func pinLightBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by replacing brighter colors.

class func saturationBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends the colors and saturation values of two images.

class func screenBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors of two images by multiplying colors.

class func softLightBlendMode() -> any CIFilter &amp; CICompositeOperation

Blurs the colors of two images by calculating luminance.

class func sourceAtopCompositing() -> any CIFilter &amp; CICompositeOperation

Overlaps two images to create one cropped image.

class func sourceInCompositing() -> any CIFilter &amp; CICompositeOperation

Subtracts non-overlapping areas of two images, resulting in one image.

class func sourceOutCompositing() -> any CIFilter &amp; CICompositeOperation

Subtracts overlapping area of two images to create the output image.

class func sourceOverCompositing() -> any CIFilter &amp; CICompositeOperation

Places one image over a second image.

class func subtractBlendMode() -> any CIFilter &amp; CICompositeOperation

Blends colors by subtracting color values from two images.

class func vividLightBlendMode() -> any CIFilter &amp; CICompositeOperation

A combination of color-burn and color-dodge blend modes.

## See Also

### Filter Catalog

Blur Filters

Apply blurs, simulate motion and zoom effects, reduce noise, and erode and dilate image regions.

Color Adjustment Filters

Apply color transformations, including exposure, hue, and tint adjustments.

Color Effect Filters

Apply color effects, including photo effects, dithering, and color maps.

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

