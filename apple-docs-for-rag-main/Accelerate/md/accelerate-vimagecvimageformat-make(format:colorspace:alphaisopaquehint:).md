

- Accelerate
- vImageCVImageFormat
-  make(format:colorSpace:alphaIsOpaqueHint:) 

Type Method

# make(format:colorSpace:alphaIsOpaqueHint:)

Creates the description of an RGB image encoding in a Core Video pixel buffer from the specified properties.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func make(
    format: vImageCVImageFormat.Format,
    colorSpace: CGColorSpace,
    alphaIsOpaqueHint: Bool
) -> vImageCVImageFormat?
```

## Parameters 

`format`  

The format type of the image.

`colorSpace`  

The color space of RGB and monochrome images.

`alphaIsOpaqueHint`  

A hint that indicates that the function interprets an image with an alpha channel as opaque.

## Return Value

A vImageCVImageFormat instance encoded with the function’s parameters.

## See Also

### Related Documentation

func vImageCVImageFormat_Create(UInt32, UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!, CFString!, CGColorSpace!, Int32) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

### Creating a Core Video image format

static func make(buffer: CVPixelBuffer) -> vImageCVImageFormat?

Creates the description of the image encoding in an existing Core Video pixel buffer.

static func make(format: vImageCVImageFormat.Format, matrix: vImage_ARGBToYpCbCrMatrix, chromaSiting: vImageCVImageFormat.ChromaSiting, colorSpace: CGColorSpace, alphaIsOpaqueHint: Bool) -> vImageCVImageFormat?

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

