

- Accelerate
- vImage
- vImage.PixelBuffer
-  unpremultiply(channelOrdering:) 

Instance Method

# unpremultiply(channelOrdering:)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unpremultiply(channelOrdering: vImage.ChannelOrdering)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`channelOrdering`  

The channel ordering of the source buffer.

## Discussion

This function divides the color values in each pixel `self` by the corresponding alpha value and copies the alpha value to the destination unchanged. The function treats the values `0 ... 255` in the pixel buffer as the values `0 ... 1`.

For example, the following code divides the RGB values `[32, 64, 128]` by the alpha value `128` (interpreted as `0.5`):

```
let src = vImage.PixelBuffer(
    pixelValues: [127, 32, 64, 128],
    size: vImage.Size(width: 1, height: 1))

src.unpremultiply(channelOrdering: .ARGB)

// Prints "[127, 64, 129, 255]".
print(src.array)
```

## See Also

### Unpremultiply

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

