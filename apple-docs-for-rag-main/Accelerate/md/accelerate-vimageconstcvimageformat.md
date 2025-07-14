

- Accelerate
-  vImageConstCVImageFormat 

Class

# vImageConstCVImageFormat

An immutable description of image encoding in a Core Video pixel buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class vImageConstCVImageFormat
```

## Discussion

Use vImageCVImageFormat_Copy(_:) to create a mutable copy of a vImageConstCVImageFormat instance.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Creating Core Video image formats

class vImageCVImageFormat

A mutable description of image encoding in a Core Video pixel buffer.

func vImageCVImageFormat_CreateWithCVPixelBuffer(CVPixelBuffer!) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of the image encoding in an existing Core Video pixel buffer.

func vImageCVImageFormat_Create(UInt32, UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!, CFString!, CGColorSpace!, Int32) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

