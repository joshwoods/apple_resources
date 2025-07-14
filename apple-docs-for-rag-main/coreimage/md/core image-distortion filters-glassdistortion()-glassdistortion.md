

- Core Image
- Distortion Filters
-  glassDistortion() 

Type Method

# glassDistortion()

Distorts an image by applying a glass-like texture.

iOS 14.0+iPadOS 14.0+Mac Catalyst 17.5+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func glassDistortion() -> any CIFilter & CIGlassDistortion
```

## Return Value

The distorted image.

## Discussion

This method applies the glass distortion filter to an image. This effect distorts an image by applying a glass texture from the raised portions of the texture map image.

The glass distortion filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`texture`  
An image with the type `CIImage`.

`scale`  
The amount of texturing to apply. Larger values increase the effect. Defaults to 200.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

The following code creates a filter that results in a glass-like distortion applied to the image:

func glassDistortion(inputImage: CIImage, textureImage: CIImage) -> CIImage {
    let filter = CIFilter.glassDistortion()
    filter.inputImage = inputImage
    filter.textureImage = textureImage
    filter.center = CGPoint(x: 1791, y: 1344)
    filter.scale = 500
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

