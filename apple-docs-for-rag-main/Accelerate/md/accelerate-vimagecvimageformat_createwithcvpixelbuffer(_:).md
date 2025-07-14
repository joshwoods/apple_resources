

- Accelerate
-  vImageCVImageFormat_CreateWithCVPixelBuffer(\_:) 

Function

# vImageCVImageFormat_CreateWithCVPixelBuffer(\_:)

Creates the description of the image encoding in an existing Core Video pixel buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_CreateWithCVPixelBuffer(_ buffer: CVPixelBuffer!) -> Unmanaged!
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

static func make(buffer: CVPixelBuffer) -> vImageCVImageFormat?

Creates the description of the image encoding in an existing Core Video pixel buffer.

### Creating Core Video image formats

class vImageCVImageFormat

A mutable description of image encoding in a Core Video pixel buffer.

class vImageConstCVImageFormat

An immutable description of image encoding in a Core Video pixel buffer.

func vImageCVImageFormat_Create(UInt32, UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!, CFString!, CGColorSpace!, Int32) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

