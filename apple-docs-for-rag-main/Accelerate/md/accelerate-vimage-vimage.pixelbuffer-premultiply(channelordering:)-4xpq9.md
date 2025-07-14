

- Accelerate
- vImage
- vImage.PixelBuffer
-  premultiply(channelOrdering:) 

Instance Method

# premultiply(channelOrdering:)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func premultiply(channelOrdering: vImage.ChannelOrdering)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`channelOrdering`  

The channel ordering of the source buffer.

## Discussion

This function multiplies the color values in each pixel `self` by the corresponding alpha value and copies the alpha value to the destination unchanged. The function treats the values `0 ... 255` in the pixel buffer as the values `0 ... 1`.

For example, the following code multiplies the RGB values `[32, 64, 128]` by the alpha value `128` (interpreted as `0.5`):

```
let src = vImage.PixelBuffer(
    pixelValues: [127, 32, 64, 128],
    size: vImage.Size(width: 1, height: 1))

src.premultiply(channelOrdering: .ARGB)

// Prints "[127, 16, 32, 64]".
print(src.array)
```

## See Also

### Premultiply

func premultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a floating-point 32-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

