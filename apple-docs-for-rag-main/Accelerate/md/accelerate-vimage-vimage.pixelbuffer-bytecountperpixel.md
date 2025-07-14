

- Accelerate
- vImage
- vImage.PixelBuffer
-  byteCountPerPixel 

Instance Property

# byteCountPerPixel

Returns the number of bytes per pixel.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var byteCountPerPixel: Int { get }
```

Available when `Format` conforms to `StaticPixelFormat`.

## Discussion

For example, the following code prints the number of bytes per pixel in two interleaved buffers:

```
 let x = vImage.PixelBuffer(size: vImage.Size(width: 1,
                                                                     height: 1))
 let y = vImage.PixelBuffer(size: vImage.Size(width: 1,
                                                                     height: 1))

 // Prints "8 4".
 print(x.byteCountPerPixel, y.byteCountPerPixel)
```

## See Also

### Inspecting a pixel buffer

var width: Int

The width of the pixel buffer.

var height: Int

The height of the pixel buffer.

var size: vImage.Size

The size of the pixel buffer.

var channelCount: Int

Returns the number of channels.

var rowStride: Int

The width, in pixels, of the underlying memory, including any additional row byte padding.

var count: Int

The total number of pixels multiplied by the number of channels in the buffer, including any row padding.

var array: [Format.ComponentType]

An array of `width * height * channelCount` values that’s a copy of the buffer’s visible contents.

