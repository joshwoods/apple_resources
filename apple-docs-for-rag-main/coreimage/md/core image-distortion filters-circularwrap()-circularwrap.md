

- Core Image
- Distortion Filters
-  circularWrap() 

Type Method

# circularWrap()

Distorts an image by increasing the distance of the center of the image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 17.5+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func circularWrap() -> any CIFilter & CICircularWrap
```

## Return Value

The distorted image.

## Discussion

This method applies the circular wrap filter to an image. This effect wraps an image around a transparent circle. The distortion of the image increases with the distance from the center of the circle.

The circular wrap filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`angle`  
A `float` representing the angle of the wrap, in radians, as an NSNumber.

`radius`  
A `float` representing the amount of pixels the filter uses to create the distortion as an `NSNumber`.

`center`  
A set of coordinates marking the center of the image as a CGPoint.

The following code creates a filter that results in a circular image generated from the input image:

func circularWrap(inputImage: CIImage) -> CIImage {    let filter = CIFilter.circularWrap()
    filter.inputImage = inputImage
    filter.center = CGPoint(
        x: inputImage.extent.size.width/2,
        y: inputImage.extent.size.height/2
    )
    filter.angle = .pi
    filter.radius = 90
    return filter.outputImage!
}

let text = CIFilter.textImageGenerator()
text.text = &quot;Core Image&quot;
text.fontSize = 100
text.fontName = &quot;Chalkboard&quot;
text.outputImage!
circularWrap(inputImage: text.outputImage!)

## See Also

### Filters

class func bumpDistortion() -> any CIFilter &amp; CIBumpDistortion

Distorts an image with a concave or convex bump.

class func bumpDistortionLinear() -> any CIFilter &amp; CIBumpDistortionLinear

Linearly distorts an image with a concave or convex bump.

class func circleSplashDistortion() -> any CIFilter &amp; CICircleSplashDistortion

Distorts an image with radiating circles to the periphery of the image.

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

