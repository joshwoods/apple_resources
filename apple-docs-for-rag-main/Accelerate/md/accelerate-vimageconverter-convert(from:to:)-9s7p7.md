

- Accelerate
- vImageConverter
-  convert(from:to:) 

Instance Method

# convert(from:to:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(
    from source: vImage.PixelBuffer,
    to destination: vImage.PixelBuffer
) throws where Src : SinglePlanePixelFormat, Dest : SinglePlanePixelFormat
```

## Mentioned in 

Building a basic image conversion workflow

## See Also

### Instance Methods

func convert(source: vImage_Buffer, destination: inout vImage_Buffer, flags: vImage.Options) throws

Converts the pixels in a vImage buffer to another format.

func mustOperateOutOfPlace(source: vImage_Buffer, destination: vImage_Buffer, flags: vImage.Options) throws -> Bool

Determines whether a converter is capable of operating in place.

func destinationBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage destination buffer types, specifying the order of planes.

func sourceBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage source buffer types, specifying the order of planes.

func convert&lt;F1, F2>(from: [vImage.PixelBuffer&lt;F1>], to: [vImage.PixelBuffer&lt;F2>]) throws

func makeCGToCVPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

func makeCVToCGPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

