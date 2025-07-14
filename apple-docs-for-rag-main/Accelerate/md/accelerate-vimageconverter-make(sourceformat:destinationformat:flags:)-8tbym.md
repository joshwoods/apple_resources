

- Accelerate
- vImageConverter
-  make(sourceFormat:destinationFormat:flags:) 

Type Method

# make(sourceFormat:destinationFormat:flags:)

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func make(
    sourceFormat: vImage_CGImageFormat,
    destinationFormat: vImage_CGImageFormat,
    flags options: vImage.Options = .noFlags
) throws -> vImageConverter
```

## Mentioned in 

Building a basic image conversion workflow

## See Also

### Related Documentation

func vImageConverter_CreateWithCGImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

### Type Methods

static func make(sourceFormat: vImageCVImageFormat, destinationFormat: vImage_CGImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImageCVImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImage_CGImageFormat, colorConversionInfo: CGColorConversionInfo) throws -> vImageConverter

