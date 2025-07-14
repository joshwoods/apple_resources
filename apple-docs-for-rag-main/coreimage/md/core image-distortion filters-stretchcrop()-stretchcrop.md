

- Core Image
- Distortion Filters
-  stretchCrop() 

Type Method

# stretchCrop()

Distorts an image by stretching or cropping to fit a specified size.

iOS 14.0+iPadOS 14.0+Mac Catalyst 17.5+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func stretchCrop() -> any CIFilter & CIStretchCrop
```

## Return Value

The distorted image.

## Discussion

This method applies the stretch crop filter to an image. This effect distorts an image by stretching an image and then applies the crop extent. If the crop value is 0, the filter only uses stretching. If the value is 1, then the filter only uses cropping.

The stretch crop filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`centerStretchAmount`  
A `float` representing the amount of stretching of the center of the image as an NSNumber.

`size`  
A CGPoint representing the desired size of the output image.

`cropAmount`  
A `float` representing the amount of cropping you apply to achieve the target size as an `NSNumber`.

The following code creates a filter that results in a smaller image that’s distorted and cropped to be the defined size:

func stretchCrop(inputImage: CIImage) -> CIImage {
    let filter = CIFilter.stretchCrop()
    filter.inputImage = inputImage
    filter.cropAmount = 0.25
    filter.centerStretchAmount = 0.25
    filter.size = CGPoint(
        x: inputImage.extent.width * 2,
        y: inputImage.extent.size.height * 0.8
    )
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

class func ninePartTiled() -> any CIFilter &amp; CINinePartTiled

Distorts an image by tiling portions of it.

class func pinchDistortion() -> any CIFilter &amp; CIPinchDistortion

Distorts an image by creating a pinch effect with stronger distortion in the center.

class func torusLensDistortion() -> any CIFilter &amp; CITorusLensDistortion

Creates a torus-shaped lens to distort the image.

class func twirlDistortion() -> any CIFilter &amp; CITwirlDistortion

Distorts an image by rotating pixels around a center point.

class func vortexDistortion() -> any CIFilter &amp; CIVortexDistortion

Distorts an image by using a vortex effect created by rotating pixels around a point.

