

- Core Image
- Geometry Adjustment Filters
-  bicubicScaleTransform() 

Type Method

# bicubicScaleTransform()

Produces a high-quality scaled version of an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func bicubicScaleTransform() -> any CIFilter & CIBicubicScaleTransform
```

## Return Value

The adjusted image.

## Discussion

This method applies the bicubic scale transform filter to an image. The effect produces a high-quality, scaled version of the input image. The parameters of `B` and `C` determine the sharpness and softness of the resampling.

The bicubic scale transform filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`aspectRatio`  
A `float` representing the aspect ratio as an NSNumber.

`parameterB`  
A `float` representing the value of B used for cubic resampling as an `NSNumber`.

`parameterC`  
A `float` representing the value of C used for cubic resampling as an `NSNumber`.

The following code creates a filter that results in the image becoming square:

func bicubicScale(inputImage: CIImage) -> CIImage {
    let bicubicScaleFilter = CIFilter.bicubicScaleTransform()
    bicubicScaleFilter.inputImage = inputImage
    bicubicScaleFilter.aspectRatio = 0.7
    bicubicScaleFilter.parameterB = 1
    bicubicScaleFilter.parameterC = 0.75
    return bicubicScaleFilter.outputImage!
}

## See Also

### Filters

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

class func straighten() -> any CIFilter &amp; CIStraighten

Rotates and crops an image.

