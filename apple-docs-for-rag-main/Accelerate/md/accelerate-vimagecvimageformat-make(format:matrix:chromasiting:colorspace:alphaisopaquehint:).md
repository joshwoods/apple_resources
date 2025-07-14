

- Accelerate
- vImageCVImageFormat
-  make(format:matrix:chromaSiting:colorSpace:alphaIsOpaqueHint:) 

Type Method

# make(format:matrix:chromaSiting:colorSpace:alphaIsOpaqueHint:)

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func make(
    format: vImageCVImageFormat.Format,
    matrix: vImage_ARGBToYpCbCrMatrix,
    chromaSiting: vImageCVImageFormat.ChromaSiting,
    colorSpace: CGColorSpace,
    alphaIsOpaqueHint: Bool
) -> vImageCVImageFormat?
```

## Parameters 

`format`  

The format type of the image.

`matrix`  

A vImage_ARGBToYpCbCrMatrix that describes the conversion from RGB to the YpCbCr format.

`chromaSiting`  

The chrominance location.

`colorSpace`  

The color space of RGB and monochrome images. For YpCbCr images, this is the color space of the RGB image before conversion to YpCbCr using the ARGB-to-YpCbCr conversion matrix. The YpCbCr format RGB primaries and transfer function define the color space.

`alphaIsOpaqueHint`  

A hint that indicates that the function interprets an image with an alpha channel as opaque.

## Return Value

A vImageCVImageFormat instance encoded with the function’s parameters.

## Discussion

This function derives values that parameters from the image format type don’t specify, such as the number of channels, channel names, and channel descriptions.

## See Also

### Related Documentation

func vImageCVImageFormat_Create(UInt32, UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!, CFString!, CGColorSpace!, Int32) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

### Creating a Core Video image format

static func make(buffer: CVPixelBuffer) -> vImageCVImageFormat?

Creates the description of the image encoding in an existing Core Video pixel buffer.

static func make(format: vImageCVImageFormat.Format, colorSpace: CGColorSpace, alphaIsOpaqueHint: Bool) -> vImageCVImageFormat?

Creates the description of an RGB image encoding in a Core Video pixel buffer from the specified properties.

