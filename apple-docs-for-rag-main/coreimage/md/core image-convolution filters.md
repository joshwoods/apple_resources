

- Core Image
-  Convolution Filters 

API Collection

# Convolution Filters

Produce effects such as blurring, sharpening, edge detection, translation, and embossing.

## Overview

A convolution filter generates each output pixel by summing all elements in the element-wise product of two matrices - the weight matrix and a matrix containing the neighbors of each input pixel. A bias is added to this and the resulting value is clamped to between 0.0 and 1.0. This operation is performed independently for each color component (including the alpha component). You can create many types of image processing effects using different weight matrices, such as blurring, sharpening, edge detection, translation, and embossing.

## Topics

### Filters

class func convolution3X3() -> any CIFilter &amp; CIConvolution

Applies a convolution 3 x 3 filter to the `RGBA` components of an image.

class func convolution5X5() -> any CIFilter &amp; CIConvolution

Applies a convolution 5 x 5 filter to the `RGBA` components image.

class func convolution7X7() -> any CIFilter &amp; CIConvolution

Applies a convolution 7 x 7 filter to the `RGBA` color components of an image.

class func convolution9Horizontal() -> any CIFilter &amp; CIConvolution

Applies a convolution-9 horizontal filter to the `RGBA` components of an image.

class func convolution9Vertical() -> any CIFilter &amp; CIConvolution

Applies a convolution-9 vertical filter to the `RGBA` components of an image.

class func convolutionRGB3X3() -> any CIFilter &amp; CIConvolution

Applies a convolution 3 x 3 filter to the `RGB` components of an image.

class func convolutionRGB5X5() -> any CIFilter &amp; CIConvolution

Applies a convolution 5 x 5 filter to the `RGB` components of an image.

class func convolutionRGB7X7() -> any CIFilter &amp; CIConvolution

Applies a convolution 7 x 7 filter to the RGB components of an image.

class func convolutionRGB9Horizontal() -> any CIFilter &amp; CIConvolution

Applies a convolution 9 x 1 filter to the RGB components of an image.

class func convolutionRGB9Vertical() -> any CIFilter &amp; CIConvolution

Applies a convolution 1 x 9 filter to the RGB components of an image.

## See Also

### Filter Catalog

Blur Filters

Apply blurs, simulate motion and zoom effects, reduce noise, and erode and dilate image regions.

Color Adjustment Filters

Apply color transformations, including exposure, hue, and tint adjustments.

Color Effect Filters

Apply color effects, including photo effects, dithering, and color maps.

Composite Operations

Composite images by using a range of blend modes and compositing operators.

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

