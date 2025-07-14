

- Core Image
- Geometry Adjustment Filters
-  straighten() 

Type Method

# straighten()

Rotates and crops an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func straighten() -> any CIFilter & CIStraighten
```

## Return Value

The adjusted image.

## Discussion

This method applies the straighten filter to an image. The effect rotates the image based on the `angle` property while cropping and scaling the image to remain the same size as the original image.

The straighten filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`angle`  
A `float` representing the angle to rotate the image as an NSNumber.

The following code creates a filter that rotates the image 135 degrees:

func straighten(inputImage: CIImage) -> CIImage {
    let straightenFilter = CIFilter.straighten()
    straightenFilter.inputImage = inputImage
    straightenFilter.angle = 135
    return straightenFilter.outputImage!
}

## See Also

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

