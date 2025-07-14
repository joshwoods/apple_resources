

- Core Image
- Geometry Adjustment Filters
-  lanczosScaleTransform() 

Type Method

# lanczosScaleTransform()

Creates a high-quality, scaled version of a source image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func lanczosScaleTransform() -> any CIFilter & CILanczosScaleTransform
```

## Return Value

The adjusted image.

## Discussion

This method applies the Lanczos scale transform filter to an image. The effect creates the output image by scaling the input image based on the scale and aspect ratio properties provided.

The Lanczos scale filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`scale`  
A `float` representing the scaling factor used on the image as an `NSNumber`. Values less than `1.0` scale down the images. Values grater than `1.0` scale up the image.

`aspectRatio`  
A `float` representing the additional horizontal scaling factor used on the image as an `NSNumber`.

The following code creates a filter that results in a smaller scaled image with high quality:

func lanczosScale(inputImage: CIImage) -> CIImage {    
    let lanczosScaleFilter = CIFilter.lanczosScaleTransform()
    lanczosScaleFilter.inputImage = inputImage
    lanczosScaleFilter.scale =  0.3
    lanczosScaleFilter.aspectRatio = 1
    return lanczosScaleFilter.outputImage!
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

