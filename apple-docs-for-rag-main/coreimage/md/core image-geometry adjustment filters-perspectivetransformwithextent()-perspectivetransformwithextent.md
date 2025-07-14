

- Core Image
- Geometry Adjustment Filters
-  perspectiveTransformWithExtent() 

Type Method

# perspectiveTransformWithExtent()

Alters an image’s geometry to adjust the perspective while applying constraints.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func perspectiveTransformWithExtent() -> any CIFilter & CIPerspectiveTransformWithExtent
```

## Return Value

The adjusted image.

## Discussion

This method applies the perspective transform with extent filter to an image. The effect alters the geometry of an image to simulate the observer changing viewing position. The extent filter crops the image within the bounds specified. You can use the perspective filter to skew an image.

The perspective transform with extent filter uses the following properties:

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

`extent`  
A CGRect representing the dimensions of the output image.

The following code creates a filter that changes the perspective of the input image:

func perspectiveTransformWithExtent(inputImage: CIImage) -> CIImage {
    let perspectiveTransformFilter = CIFilter.perspectiveTransformWithExtent()
    perspectiveTransformFilter.inputImage = inputImage
    perspectiveTransformFilter.topLeft = CGPoint(x: 100, y: 3984)
    perspectiveTransformFilter.topRight = CGPoint(x: 3732, y: 3025)
    perspectiveTransformFilter.bottomLeft = CGPoint(x: 0, y: 500)
    perspectiveTransformFilter.bottomRight = CGPoint(x: 4032, y: 120)
    perspectiveTransformFilter.extent = CGRect(x: 0, y: 0, width: 3800, height: 3200)
    return perspectiveTransformFilter.outputImage!
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

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

