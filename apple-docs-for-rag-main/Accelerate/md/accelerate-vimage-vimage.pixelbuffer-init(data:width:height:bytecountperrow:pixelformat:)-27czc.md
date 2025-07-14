

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(data:width:height:byteCountPerRow:pixelFormat:) 

Initializer

# init(data:width:height:byteCountPerRow:pixelFormat:)

Calculates the correct bytes per row and returns a new buffer that references existing data.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    data: UnsafeMutableRawPointer,
    width: Int,
    height: Int,
    byteCountPerRow: Int? = nil,
    pixelFormat: Format.Type = Format.self
)
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`data`  

A pointer to the top-left pixel of the buffer.

`width`  

The width, in pixels, of the pixel buffer.

`height`  

The height, in pixels, of the pixel buffer.

`byteCountPerRow`  

The number of bytes in a pixel row.

`pixelFormat`  

The pixel format of the initialized buffer.

## Discussion

Pass `nil` to `byteCountPerRow` to have the function calculate the bytes per row as `width * MemoryLayout.stride * T.channelCount`.

For example, the following code creates a 32-bit planar pixel buffer:

```
 let data = UnsafeMutableBufferPointer.allocate(capacity: 10)
 _ = data.initialize(from: [0, 1, 2, 3, 4,
                            5, 6, 7, 8, 9] as [Float])
 defer {
     data.deallocate()
 }

 let src = vImage.PixelBuffer(data: data.baseAddress!,
                              width: 5,
                              height: 2,
                              byteCountPerRow: nil,
                              pixelFormat: vImage.PlanarF.self)

 // Prints "[0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0]"
 print(src.array)
```

Important

The pixel buffer is valid only for the lifetime of `data`.

## See Also

### Creating a pixel buffer from raw pixel data

init&lt;U>(pixelValues: U, size: vImage.Size, pixelFormat: Format.Type)

Creates a new pixel buffer by copying the supplied collection of pixel values.

init(data: UnsafeMutableRawPointer, width: Int, height: Int, byteCountPerRow: Int, pixelFormat: Format.Type)

Returns a new buffer that references existing data.

