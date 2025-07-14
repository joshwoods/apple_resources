

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(pixelValues:size:pixelFormat:) 

Initializer

# init(pixelValues:size:pixelFormat:)

Creates a new pixel buffer by copying the supplied collection of pixel values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    pixelValues: U,
    size: vImage.Size,
    pixelFormat: Format.Type = Format.self
) where U : AccelerateBuffer, Format.ComponentType == U.Element
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`pixelValues`  

The source pixel values. `pixelValues` must contain `size.width * size.height * channelCount` elements.

`size`  

The size of the new buffer.

`pixelFormat`  

The pixel format of the initialized buffer.

## Discussion

## See Also

### Creating a pixel buffer from raw pixel data

init(data: UnsafeMutableRawPointer, width: Int, height: Int, byteCountPerRow: Int, pixelFormat: Format.Type)

Returns a new buffer that references existing data.

init(data: UnsafeMutableRawPointer, width: Int, height: Int, byteCountPerRow: Int?, pixelFormat: Format.Type)

Calculates the correct bytes per row and returns a new buffer that references existing data.

