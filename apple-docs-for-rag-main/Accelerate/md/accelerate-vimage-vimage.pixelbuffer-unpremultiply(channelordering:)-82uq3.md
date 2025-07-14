

- Accelerate
- vImage
- vImage.PixelBuffer
-  unpremultiply(channelOrdering:) 

Instance Method

# unpremultiply(channelOrdering:)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unpremultiply(channelOrdering: vImage.ChannelOrdering)
```

Available when `Format` is `vImage.InterleavedFx4`.

## Parameters 

`channelOrdering`  

The channel ordering of the source buffer.

## Discussion

This function divides the color values in each pixel `self` by the corresponding alpha value and copies the alpha value to the destination unchanged.

For example, the following code divides the RGB values `[0.125, 0.25, 0.5]` by the alpha value `0.5`:

```
let src = vImage.PixelBuffer(
    pixelValues: [0.5,
                  0.125, 0.25, 0.5],
    size: vImage.Size(width: 1, height: 1))

src.unpremultiply(channelOrdering: .ARGB)

// Prints "[0.5, 0.25, 0.5, 1.0]"
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

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

