

- Core Image
- Geometry Adjustment Filters
-  perspectiveCorrection() 

Type Method

# perspectiveCorrection()

Transforms an image’s perspective.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func perspectiveCorrection() -> any CIFilter & CIPerspectiveCorrection
```

## Return Value

The adjusted image.

## Discussion

This method applies the perspective correction filter to an image. The effect applies a perspective correction transforming nonrectangular area in the source image to a rectangular output image.

The perspective correction filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`topLeft`  
A CGPoint in the input image mapped to the top-left corner of the output image.

`topRight`  
A `CGPoint` in the input image mapped to the top-right corner of the output image.

`bottomLeft`  
A `CGPoint` in the input image mapped to the bottom-left corner of the output image.

`bottomRight`  
A `CGPoint` in the input image mapped to the bottom-right corner of the output image.

The following code creates a filter that corrects the perspective to appear straight:

func perspectiveCorrection(inputImage: CIImage) -> CIImage {
    let perspectiveCorrectionFilter = CIFilter.perspectiveCorrection()
    perspectiveCorrectionFilter.inputImage = inputImage
    perspectiveCorrectionFilter.topRight = CGPoint(x: 0, y: 3024)
    perspectiveCorrectionFilter.topLeft = CGPoint(x: 4032, y: 3024)
    perspectiveCorrectionFilter.bottomRight = CGPoint(x: 200, y: 0)
    perspectiveCorrectionFilter.bottomLeft = CGPoint(x: 4032, y: 0)
    return perspectiveCorrectionFilter.outputImage!
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

class func perspectiveRotate() -> any CIFilter &amp; CIPerspectiveRotate

Rotates an image in a 3D space.

class func perspectiveTransform() -> any CIFilter &amp; CIPerspectiveTransform

Alters an image’s geometry to adjust the perspective.

class func perspectiveTransformWithExtent() -> any CIFilter &amp; CIPerspectiveTransformWithExtent

Alters an image’s geometry to adjust the perspective while applying constraints.

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

