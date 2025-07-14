

- Accelerate
- vImage
- vImage.PixelBuffer
-  makePixelBufferAndCGImageFormat(cgImage:pixelFormat:) 

Type Method

# makePixelBufferAndCGImageFormat(cgImage:pixelFormat:)

Returns a new pixel buffer and Core Graphics image format structure from a Core Graphics image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func makePixelBufferAndCGImageFormat(
    cgImage: CGImage,
    pixelFormat: Format.Type = Format.self
) throws -> (pixelBuffer: vImage.PixelBuffer, cgImageFormat: vImage_CGImageFormat)
```

Available when `Format` conforms to `InitializableFromCGImage` and `StaticPixelFormat`.

## Parameters 

`cgImage`  

The source Core Graphics image.

`pixelFormat`  

The pixel format of the initialized buffer.

## Return Value

A new pixel buffer of type vImage.DynamicPixelFormat and a vImage_CGImageFormat that describes the ordering and number of the color channels, the size and type of the data in the color channels, and whether or not the data is premultiplied by alpha.

## Discussion

Use this function where you know the bits per component and bits per pixel of the CGImage instance. These must match those of the buffer’s `pixelFormat`, otherwise this function returns `nil`.

## See Also

### Creating a pixel buffer and image format

static func makeDynamicPixelBufferAndCGImageFormat(cgImage: CGImage) throws -> (pixelBuffer: vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>, cgImageFormat: vImage_CGImageFormat)

Returns a new dynamic pixel format pixel buffer and Core Graphics image format structure from a Core Graphics image.

