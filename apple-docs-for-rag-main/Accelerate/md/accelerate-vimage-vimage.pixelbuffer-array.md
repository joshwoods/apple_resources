

- Accelerate
- vImage
- vImage.PixelBuffer
-  array 

Instance Property

# array

An array of `width * height * channelCount` values that’s a copy of the buffer’s visible contents.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var array: [Format.ComponentType] { get }
```

Available when `Format` conforms to `StaticPixelFormat`.

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

var byteCountPerPixel: Int

Returns the number of bytes per pixel.

var count: Int

The total number of pixels multiplied by the number of channels in the buffer, including any row padding.

