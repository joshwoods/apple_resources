

- Accelerate
- vImageConverter
-  convert(from:to:) 

Instance Method

# convert(from:to:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(
    from sources: [vImage.PixelBuffer],
    to destinations: [vImage.PixelBuffer]
) throws where F1 : SinglePlanePixelFormat, F2 : SinglePlanePixelFormat
```

## Mentioned in 

Converting chroma-subsampled images

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

func convert&lt;Src, Dest>(from: vImage.PixelBuffer&lt;Src>, to: vImage.PixelBuffer&lt;Dest>) throws

func makeCGToCVPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

func makeCVToCGPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

