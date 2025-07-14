

- Accelerate
- vImageConverter
-  make(sourceFormat:destinationFormat:colorConversionInfo:) 

Type Method

# make(sourceFormat:destinationFormat:colorConversionInfo:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func make(
    sourceFormat: vImage_CGImageFormat,
    destinationFormat: vImage_CGImageFormat,
    colorConversionInfo: CGColorConversionInfo
) throws -> vImageConverter
```

## See Also

### Type Methods

static func make(sourceFormat: vImageCVImageFormat, destinationFormat: vImage_CGImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImage_CGImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImageCVImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

