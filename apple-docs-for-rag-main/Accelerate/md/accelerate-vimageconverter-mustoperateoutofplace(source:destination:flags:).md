

- Accelerate
- vImageConverter
-  mustOperateOutOfPlace(source:destination:flags:) 

Instance Method

# mustOperateOutOfPlace(source:destination:flags:)

Determines whether a converter is capable of operating in place.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func mustOperateOutOfPlace(
    source: vImage_Buffer,
    destination: vImage_Buffer,
    flags options: vImage.Options = .noFlags
) throws -> Bool
```

## See Also

### Related Documentation

func vImageConverter_MustOperateOutOfPlace(vImageConverter, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Determines whether a converter is capable of operating in place.

### Instance Methods

func convert(source: vImage_Buffer, destination: inout vImage_Buffer, flags: vImage.Options) throws

Converts the pixels in a vImage buffer to another format.

func destinationBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage destination buffer types, specifying the order of planes.

func sourceBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage source buffer types, specifying the order of planes.

func convert&lt;Src, Dest>(from: vImage.PixelBuffer&lt;Src>, to: vImage.PixelBuffer&lt;Dest>) throws

func convert&lt;F1, F2>(from: [vImage.PixelBuffer&lt;F1>], to: [vImage.PixelBuffer&lt;F2>]) throws

func makeCGToCVPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

func makeCVToCGPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

