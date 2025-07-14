

- Accelerate
- vImageConverter
-  convert(source:destination:flags:) 

Instance Method

# convert(source:destination:flags:)

Converts the pixels in a vImage buffer to another format.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func convert(
    source: vImage_Buffer,
    destination: inout vImage_Buffer,
    flags options: vImage.Options = .noFlags
) throws
```

## Mentioned in 

Building a basic image conversion workflow

## See Also

### Related Documentation

func vImageConvert_AnyToAny(vImageConverter, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Converts the pixels in a vImage buffer to another format, using the specified converter.

### Instance Methods

func mustOperateOutOfPlace(source: vImage_Buffer, destination: vImage_Buffer, flags: vImage.Options) throws -> Bool

Determines whether a converter is capable of operating in place.

func destinationBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage destination buffer types, specifying the order of planes.

func sourceBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage source buffer types, specifying the order of planes.

func convert&lt;Src, Dest>(from: vImage.PixelBuffer&lt;Src>, to: vImage.PixelBuffer&lt;Dest>) throws

func convert&lt;F1, F2>(from: [vImage.PixelBuffer&lt;F1>], to: [vImage.PixelBuffer&lt;F2>]) throws

func makeCGToCVPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

func makeCVToCGPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

