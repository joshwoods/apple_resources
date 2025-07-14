

- Core Image
- Distortion Filters
-  ninePartTiled() 

Type Method

# ninePartTiled()

Distorts an image by tiling portions of it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 17.5+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func ninePartTiled() -> any CIFilter & CINinePartTiled
```

## Return Value

The distorted image.

## Discussion

This method applies the nine-part tiled filter to an image. This effect distorts an image by tiling an image based on the breakpoints properties.

The nine-part tiled filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`flipYTiles`  
A `Boolean` value representing if the y-axis should be flipped.

`growAmount`  
A CGPoint representing the amount of stretching applied.

`breakpoint1`  
A `CGPoint` representing the upper-right corner of the image to retain after tiling ends.

`breakpoint0`  
A `CGPoint` representing the lower-left corner of image to retain before stretching begins.

The following code creates a filter that results in distorted tiles of the image becoming flipped:

func ninePartTiled(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.ninePartTiled()
    filter.inputImage = inputImage
    filter.setDefaults()
    filter.breakpoint0 = CGPoint(x: 200, y: 200)
    filter.breakpoint1 = CGPoint(x: inputImage.extent.size.width-200, y: inputImage.extent.size.height - 200)
    filter.growAmount = CGPoint(x: 500, y: 500)
    return filter.outputImage!
}

## See Also

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

