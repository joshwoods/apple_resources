

- Core Image
-  Tile Effect Filters 

API Collection

# Tile Effect Filters

Produce tiled images from source images.

## Topics

### Filters

class func affineClamp() -> any CIFilter &amp; CIAffineClamp

Performs a transform on the image and extends the image edges to infinity.

class func affineTile() -> any CIFilter &amp; CIAffineTile

Performs a transform on the image and tiles the result.

class func eightfoldReflectedTile() -> any CIFilter &amp; CIEightfoldReflectedTile

Creates an eight-way reflected pattern.

class func fourfoldReflectedTile() -> any CIFilter &amp; CIFourfoldReflectedTile

Creates a four-way reflected pattern.

class func fourfoldRotatedTile() -> any CIFilter &amp; CIFourfoldRotatedTile

Creates a tiled image by rotating a tile in increments of 90 degrees.

class func fourfoldTranslatedTile() -> any CIFilter &amp; CIFourfoldTranslatedTile

Creates a tiled image by applying four translation operations.

class func glideReflectedTile() -> any CIFilter &amp; CIGlideReflectedTile

Tiles an image by rotating and reflecting a tile from the image.

class func kaleidoscope() -> any CIFilter &amp; CIKaleidoscope

Creates a 12-way kaleidoscopic image from an image.

class func opTile() -> any CIFilter &amp; CIOpTile

Produces an effect that mimics a style of visual art that uses optical illusions.

class func parallelogramTile() -> any CIFilter &amp; CIParallelogramTile

Warps the image to create a parallelogram and tiles the result.

class func perspectiveTile() -> any CIFilter &amp; CIPerspectiveTile

Tiles an image by adjusting the perspective of the image.

class func sixfoldReflectedTile() -> any CIFilter &amp; CISixfoldReflectedTile

Produces a tiled image from a source image by applying a six-way reflected symmetry.

class func sixfoldRotatedTile() -> any CIFilter &amp; CISixfoldRotatedTile

Creates a tiled image by rotating in increments of 60 degrees.

class func triangleKaleidoscope() -> any CIFilter &amp; CITriangleKaleidoscope

Create a triangular kaleidoscope effect and then tiles the result.

class func triangleTile() -> any CIFilter &amp; CITriangleTile

Tiles a triangular area of an image.

class func twelvefoldReflectedTile() -> any CIFilter &amp; CITwelvefoldReflectedTile

Creates a tiled image by rotating in increments of 30 degrees.

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

Transition Filters

Transition between two images by using effects including page curl and swipe.

