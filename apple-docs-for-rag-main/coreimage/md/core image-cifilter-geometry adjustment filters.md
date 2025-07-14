

- Core Image
- CIFilter
-  Geometry Adjustment Filters 

API Collection

# Geometry Adjustment Filters

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

### Protocols

protocol CIBicubicScaleTransform

The properties you use to configure a bicubic scale transform filter.

protocol CIEdgePreserveUpsample

The properties you use to configure an edge preserve upsample filter.

protocol CIFourCoordinateGeometryFilter

protocol CIKeystoneCorrectionCombined

protocol CIKeystoneCorrectionHorizontal

protocol CIKeystoneCorrectionVertical

protocol CILanczosScaleTransform

The properties you use to configure a Lanczos scale transform filter.

protocol CIPerspectiveCorrection

The properties you use to configure a perspective correction filter.

protocol CIPerspectiveRotate

protocol CIPerspectiveTransform

The properties you use to configure a perspective transform filter.

protocol CIPerspectiveTransformWithExtent

The properties you use to configure a perspective transform with extent filter.

protocol CIStraighten

The properties you use to configure a straighten filter.

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

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

