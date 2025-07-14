

- Core Image
- Geometry Adjustment Filters
-  perspectiveRotate() 

Type Method

# perspectiveRotate()

Rotates an image in a 3D space.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func perspectiveRotate() -> any CIFilter & CIPerspectiveRotate
```

## Return Value

The adjusted image.

## Discussion

This method applies the perspective rotate filter to an image. The effect rotates the image in 3D space to simulate the observer changing viewing position.

The perspective rotate filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`pitch`  
A `float` representing the adjustment along the pitch axis in 3D space as an NSNumber.

`yaw`  
A `float` representing the adjustment along the vertical axis as an `NSNumber`.

`roll`  
A `float` representing the amount of horizontal axis in 3D space as an `NSNumber`.

`focalLength`  
A `float` representing the simulated focal length as an `NSNumber`.

The following code creates a filter that rotates the image:

func perspectiveRotate(inputImage: CIImage) -> CIImage {
    let perspectiveRotateFilter = CIFilter.perspectiveRotate()
    perspectiveRotateFilter.inputImage = inputImage
    perspectiveRotateFilter.pitch = 0
    perspectiveRotateFilter.yaw = 0.1
    perspectiveRotateFilter.roll = 0.3
    perspectiveRotateFilter.focalLength = 18
    return perspectiveRotateFilter.outputImage!
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

class func perspectiveTransform() -> any CIFilter &amp; CIPerspectiveTransform

Alters an image’s geometry to adjust the perspective.

class func perspectiveTransformWithExtent() -> any CIFilter &amp; CIPerspectiveTransformWithExtent

Alters an image’s geometry to adjust the perspective while applying constraints.

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

