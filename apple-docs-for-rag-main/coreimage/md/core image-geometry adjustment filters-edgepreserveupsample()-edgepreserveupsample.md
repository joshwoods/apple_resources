

- Core Image
- Geometry Adjustment Filters
-  edgePreserveUpsample() 

Type Method

# edgePreserveUpsample()

Creates a high-quality upscaled image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func edgePreserveUpsample() -> any CIFilter & CIEdgePreserveUpsample
```

## Return Value

The adjusted image.

## Discussion

This method applies the edge preserve upsample filter to an image. The effect upsamples a small input image to be the size of the scale image using the luminance of the input image to preserve detail.

The edge preserve upsample filter uses the following properties:

`inputImage`  
An image representing the image to upscale with the type CIImage.

`scaleImage`  
An image representing the reference for scaling the input image with the type `CIImage`.

`spatialSigma`  
A float representing the influence of the input image’s spatial information on the upsampling operation as an NSNumber.

`lumaSimga`  
A float representing influence of the input image’s luma information on the upsampling operation as an `NSNumber`.

The following code creates a filter that upscales the smaller image to the size of the scale image:

func edgePerserveUp(inputImage: CIImage, smallImage: CIImage) -> CIImage {
    let edgePerserveUpFilter = CIFilter.edgePreserveUpsample()
    edgePerserveUpFilter.inputImage = inputImage
    edgePerserveUpFilter.smallImage = smallImage
    edgePerserveUpFilter.spatialSigma = 5
    edgePerserveUpFilter.lumaSigma = 0.15
    return edgePerserveUpFilter.outputImage!
}

## See Also

### Filters

class func bicubicScaleTransform() -> any CIFilter &amp; CIBicubicScaleTransform

Produces a high-quality scaled version of an image.

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

