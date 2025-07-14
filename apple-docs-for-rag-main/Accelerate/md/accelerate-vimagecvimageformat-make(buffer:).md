

- Accelerate
- vImageCVImageFormat
-  make(buffer:) 

Type Method

# make(buffer:)

Creates the description of the image encoding in an existing Core Video pixel buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func make(buffer: CVPixelBuffer) -> vImageCVImageFormat?
```

## Parameters 

`buffer`  

The source Core Video pixel buffer.

## Return Value

A vImageCVImageFormat instance that describes the specified pixel buffer’s pixel format.

## Mentioned in 

Converting chroma-subsampled images

## See Also

### Related Documentation

func vImageCVImageFormat_CreateWithCVPixelBuffer(CVPixelBuffer!) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of the image encoding in an existing Core Video pixel buffer.

### Creating a Core Video image format

static func make(format: vImageCVImageFormat.Format, matrix: vImage_ARGBToYpCbCrMatrix, chromaSiting: vImageCVImageFormat.ChromaSiting, colorSpace: CGColorSpace, alphaIsOpaqueHint: Bool) -> vImageCVImageFormat?

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

static func make(format: vImageCVImageFormat.Format, colorSpace: CGColorSpace, alphaIsOpaqueHint: Bool) -> vImageCVImageFormat?

Creates the description of an RGB image encoding in a Core Video pixel buffer from the specified properties.

