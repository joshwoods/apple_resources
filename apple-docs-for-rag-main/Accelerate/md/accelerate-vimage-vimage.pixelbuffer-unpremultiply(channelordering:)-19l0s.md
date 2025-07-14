

- Accelerate
- vImage
- vImage.PixelBuffer
-  unpremultiply(channelOrdering:) 

Instance Method

# unpremultiply(channelOrdering:)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unpremultiply(channelOrdering: vImage.ChannelOrdering)
```

Available when `Format` is `vImage.Interleaved16Ux4`.

## Parameters 

`channelOrdering`  

The channel ordering of the source buffer.

## Discussion

This function divides the color values in each pixel `self` by the corresponding alpha value and copies the alpha value to the destination unchanged. The function treats the values `0 ... UInt16.max` in the pixel buffer as the values `0 ... 1`.

For example, the following code divides the RGB values `[UInt16.max / 8, UInt16.max / 4, UInt16.max / 2]` by the alpha value `UInt16.max / 2`:

```
let src = vImage.PixelBuffer(
    pixelValues: [UInt16.max / 2,
                  UInt16.max / 8, UInt16.max / 4, UInt16.max / 2],
    size: vImage.Size(width: 1, height: 1))

src.unpremultiply(channelOrdering: .ARGB)

// Prints "[32767, 16383, 32767, 65535]"
//  ≅ [UInt16.max / 2, UInt16.max / 4, UInt16.max / 2, UInt16.max]
print(src.array)
```

## See Also

### Unpremultiply

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

