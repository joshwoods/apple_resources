

- Core Image
- Geometry Adjustment Filters
-  keystoneCorrectionCombined() 

Type Method

# keystoneCorrectionCombined()

Adjusts the image vertically and horizontally to remove distortion.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func keystoneCorrectionCombined() -> any CIFilter & CIKeystoneCorrectionCombined
```

## Return Value

The adjusted image.

## Discussion

This method applies the keystone correction combined filter to an image. The effect applies a combined set of horizontal and vertical guides to adjust the shape of the input image. This effect is commonly used when cropping an image to correct distortion. In the figure below, both vertical and horizontal adjustments are made, resulting in a trapezoid-shaped image.

The keystone correction filter uses the following properties:

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

`focalLength`  
A `float` representing the simulated focal length as an NSNumber.

The following code creates a filter that distorts the image:

func keystoneCorrectionCombined(inputImage: CIImage) -> CIImage {
    let keystoneCorrect = CIFilter.keystoneCorrectionCombined()
    keystoneCorrect.inputImage = inputImage
    keystoneCorrect.topLeft = CGPoint(x: 0, y: 2448)
    keystoneCorrect.topRight = CGPoint(x: 3164, y: 2248)
    keystoneCorrect.bottomLeft = CGPoint(x: 0, y: 0)
    keystoneCorrect.bottomRight = CGPoint(x: 3164, y: 150)
    keystoneCorrect.focalLength = 35
    return keystoneCorrect.outputImage!
}

## See Also

### Filters

class func bicubicScaleTransform() -> any CIFilter &amp; CIBicubicScaleTransform

Produces a high-quality scaled version of an image.

class func edgePreserveUpsample() -> any CIFilter &amp; CIEdgePreserveUpsample

Creates a high-quality upscaled image.

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

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

