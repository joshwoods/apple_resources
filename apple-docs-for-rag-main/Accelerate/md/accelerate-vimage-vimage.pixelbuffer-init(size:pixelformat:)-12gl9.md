

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(size:pixelFormat:) 

Initializer

# init(size:pixelFormat:)

Returns a new multiplane pixel buffer with a size that you specify.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    size: vImage.Size,
    pixelFormat: Format.Type = Format.self
)
```

Available when `Format` conforms to `MultiplePlanePixelFormat`.

## Parameters 

`size`  

The width and height of the buffer.

`pixelFormat`  

The pixel format of the buffer.

## Discussion

This initializer allocates but doesn’t initialize the pixel buffer’s memory. That is, the operation doesn’t guarantee that all pixel values are zero.

## See Also

### Creating a pixel buffer

init(size: vImage.Size, pixelFormat: Format.Type)

Returns a new pixel buffer with a size that you specify.

init(width: Int, height: Int, pixelFormat: Format.Type)

Returns a new pixel buffer with a width and height that you specify.

struct Size

A structure that contains width and height values.

