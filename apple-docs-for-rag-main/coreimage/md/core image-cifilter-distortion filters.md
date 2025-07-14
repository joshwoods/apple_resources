

- Core Image
- CIFilter
-  Distortion Filters 

API Collection

# Distortion Filters

## Topics

### Filters

class func bumpDistortion() -> any CIFilter &amp; CIBumpDistortion

Distorts an image with a concave or convex bump.

class func bumpDistortionLinear() -> any CIFilter &amp; CIBumpDistortionLinear

Linearly distorts an image with a concave or convex bump.

class func circleSplashDistortion() -> any CIFilter &amp; CICircleSplashDistortion

Distorts an image with radiating circles to the periphery of the image.

class func circularWrap() -> any CIFilter &amp; CICircularWrap

Distorts an image by increasing the distance of the center of the image.

class func displacementDistortion() -> any CIFilter &amp; CIDisplacementDistortion

Applies the grayscale values of the second image to the first image.

class func droste() -> any CIFilter &amp; CIDroste

Stylizes an image with the Droste effect.

class func glassDistortion() -> any CIFilter &amp; CIGlassDistortion

Distorts an image by applying a glass-like texture.

class func glassLozenge() -> any CIFilter &amp; CIGlassLozenge

Creates a lozenge-shaped lens and distorts the image.

class func holeDistortion() -> any CIFilter &amp; CIHoleDistortion

Distorts an image with a circular area that pushes the image outward.

class func lightTunnel() -> any CIFilter &amp; CILightTunnel

Distorts an image by generating a light tunnel.

class func ninePartStretched() -> any CIFilter &amp; CINinePartStretched

Distorts an image by stretching it between two breakpoints.

class func ninePartTiled() -> any CIFilter &amp; CINinePartTiled

Distorts an image by tiling portions of it.

class func pinchDistortion() -> any CIFilter &amp; CIPinchDistortion

Distorts an image by creating a pinch effect with stronger distortion in the center.

class func stretchCrop() -> any CIFilter &amp; CIStretchCrop

Distorts an image by stretching or cropping to fit a specified size.

class func torusLensDistortion() -> any CIFilter &amp; CITorusLensDistortion

Creates a torus-shaped lens to distort the image.

class func twirlDistortion() -> any CIFilter &amp; CITwirlDistortion

Distorts an image by rotating pixels around a center point.

class func vortexDistortion() -> any CIFilter &amp; CIVortexDistortion

Distorts an image by using a vortex effect created by rotating pixels around a point.

### Protocols

protocol CIBumpDistortion

protocol CIBumpDistortionLinear

protocol CICircleSplashDistortion

protocol CICircularWrap

protocol CIDisplacementDistortion

protocol CIDroste

protocol CIGlassDistortion

protocol CIGlassLozenge

protocol CIHoleDistortion

protocol CILightTunnel

protocol CINinePartStretched

protocol CINinePartTiled

protocol CIPinchDistortion

protocol CIStretchCrop

protocol CITorusLensDistortion

protocol CITwirlDistortion

protocol CIVortexDistortion

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

