

- Accelerate
- vImageConverter
-  makeCVToCGPixelBuffers(referencing:) 

Instance Method

# makeCVToCGPixelBuffers(referencing:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func makeCVToCGPixelBuffers(referencing lockedCVPixelBuffer: CVPixelBuffer) throws -> [vImage.PixelBuffer]
```

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

func convert&lt;F1, F2>(from: [vImage.PixelBuffer&lt;F1>], to: [vImage.PixelBuffer&lt;F2>]) throws

func makeCGToCVPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

