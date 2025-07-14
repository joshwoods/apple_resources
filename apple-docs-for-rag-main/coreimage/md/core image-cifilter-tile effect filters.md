

- Core Image
- CIFilter
-  Tile Effect Filters 

API Collection

# Tile Effect Filters

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

### Protocols

protocol CIAffineClamp

The properties you use to configure an affine clamp filter.

protocol CIAffineTile

The properties you use to configure an affine tile filter.

protocol CIEightfoldReflectedTile

The properties you use to configure an eightfold reflected tile filter.

protocol CIFourfoldReflectedTile

The properties you use to configure a fourfold reflected tile filter.

protocol CIFourfoldRotatedTile

The properties you use to configure a fourfold rotated tile filter.

protocol CIFourfoldTranslatedTile

The properties you use to configure a fourfold translated tile filter.

protocol CIGlideReflectedTile

The properties you use to configure a glide reflected tile filter.

protocol CIKaleidoscope

The properties you use to configure a kaleidoscope filter.

protocol CIOpTile

The properties you use to configure an optical tile filter.

protocol CIParallelogramTile

The properties you use to configure a parallelogram tile filter.

protocol CIPerspectiveTile

The properties you use to configure a perspective tile filter.

protocol CISixfoldReflectedTile

The properties you use to configure a sixfold reflected tile filter.

protocol CISixfoldRotatedTile

The properties you use to configure a sixfold rotated tile filter.

protocol CITriangleKaleidoscope

The properties you use to configure a triangle kaleidoscope filter.

protocol CITriangleTile

The properties you use to configure a triangle tile filter.

protocol CITwelvefoldReflectedTile

The properties you use to configure a twelvefold reflected tile filter.

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

Stylizing Filters

Transition Filters

