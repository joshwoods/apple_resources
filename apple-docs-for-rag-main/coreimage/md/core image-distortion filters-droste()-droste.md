

- Core Image
- Distortion Filters
-  droste() 

Type Method

# droste()

Stylizes an image with the Droste effect.

iOS 14.0+iPadOS 14.0+Mac Catalyst 17.5+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func droste() -> any CIFilter & CIDroste
```

## Return Value

The distorted image.

## Discussion

This method applies the Droste filter to an image. This effect creates a Droste effect that distorts the image by repeating smaller versions of the same image within itself.

The Droste filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`rotation`  
A `float` representing the angle of the rotation, in radians, as an NSNumber.

`zoom`  
A `float` representing the zoom of the effect as an `NSNumber`.

`periodicity`  
A float representing the amount of intervals as an `NSNumber`.

`inputInsetPoint1`  
A CGPoint representing the x and y position that defines the first inset point.

`inputInsetPoint0`  
A `CGPoint` representing the x and y position that defines the second inset point.

`inputStrands`  
A float representing the amount of strands as an `NSNumber`.

The following code creates a filter that results in the image becoming a repeated, scaled pattern:

func drosteFilter(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.droste()
    filter.inputImage = inputImage
    filter.insetPoint1 = CGPoint(
        x: inputImage.extent.size.width * 0.2,
        y: inputImage.extent.size.height * 0.2
    )
    filter.insetPoint0 = CGPoint(
        x: inputImage.extent.size.width * 0.8,
        y: inputImage.extent.size.height * 0.8
    )
    filter.periodicity = 1
    filter.rotation = 0
    filter.strands = 1
    filter.zoom = 1
    return filter.outputImage!.cropped(to: inputImage.extent)
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

