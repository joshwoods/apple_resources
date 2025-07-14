

- Core Image
-  Geometry Adjustment Filters 

API Collection

# Geometry Adjustment Filters

Translate, scale, and rotate images in 2D and 3D.

## Topics

### Filters

class func bicubicScaleTransform() -> any CIFilter &amp; CIBicubicScaleTransform

Produces a high-quality scaled version of an image.

class func edgePreserveUpsample() -> any CIFilter &amp; CIEdgePreserveUpsample

Creates a high-quality upscaled image.

class func keystoneCorrectionCombined() -> any CIFilter &amp; CIKeystoneCorrectionCombined

Adjusts the image vertically and horizontally to remove distortion.

class func keystoneCorrectionHorizontal() -> any CIFilter &amp; CIKeystoneCorrectionHorizontal

Horizontally adjusts an image to remove distortion.

class func keystoneCorrectionVertical() -> any CIFilter &amp; CIKeystoneCorrectionVertical

Vertically adjusts an image to remove distortion.

class func lanczosScaleTransform() -> any CIFilter &amp; CILanczosScaleTransform

Creates a high-quality, scaled version of a source image.

class func perspectiveCorrection() -> any CIFilter &amp; CIPerspectiveCorrection

Transforms an image’s perspective.

class func perspectiveRotate() -> any CIFilter &amp; CIPerspectiveRotate

Rotates an image in a 3D space.

class func perspectiveTransform() -> any CIFilter &amp; CIPerspectiveTransform

Alters an image’s geometry to adjust the perspective.

class func perspectiveTransformWithExtent() -> any CIFilter &amp; CIPerspectiveTransformWithExtent

Alters an image’s geometry to adjust the perspective while applying constraints.

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

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

